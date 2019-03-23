### Ethereum Casper - 認識 BLS signature

\- [7月 27, 2018](http://kimiwublog.blogspot.com/2018/07/ethereum-casper-bls-signature.html)

最近重新追了一下Ethereum Casper的進展，發現到好多新東西（應該是之前看得太表面 ＸＤ），Casper跟sharding會綁一起，然後又有個beacon chain，zk-STARK（zk-SNARK的升級版）也來湊一腳，短時間有點難消化，有興趣的人可以google上面幾個keyword。

不過，今天想要介紹的是BLS signature（這又是什麼？？？？？），這個新的簽章方式讓Casper往前再邁進一步！

BLS是Boneh–Lynn–Shacham的縮寫，有興趣的可以參考[wiki](https://en.wikipedia.org/wiki/Boneh%E2%80%93Lynn%E2%80%93Shacham)。這個簽章方式厲害的是，可以把所有signature加起來，然後驗證。如果以現今的ECDSA簽章，100個人簽同一個message，那訊息量就是乘以100倍，以Ethereum官方估計，Casper的validators約有30萬，每一個finality都需要2/3的節點做投票，光是驗證signature這件事，大概就要花到一天，所以以現行的ECDSA簽章方式根本不可行。這也是之前Casper的bottleneck之一，Ethereum的researcher, Justin Drake提出了這個[方案](https://ethresear.ch/t/pragmatic-signature-aggregation-with-bls/2105)，當然也不是拿了就可以用的，BLS的介紹可以參考[BLS signatures: better than Schnorr](https://medium.com/@snigirev.stepan/bls-signatures-better-than-schnorr-5a7fe30ea716)，寫得非常清楚也好懂。下面會簡單介紹一下。

首先，就是要找到一個特殊的橢圓對稱曲線可以達到以下的算式
e(a x P, b x Q) = e(P, ab x Q) = e(ab x P, Q) = e(P, Q)^(ab)
[![|320x247](https://cdn-images-1.medium.com/max/2000/1*IpmIdJLR36iHnOHq1OqHnw@2x.png)](https://cdn-images-1.medium.com/max/2000/1*IpmIdJLR36iHnOHq1OqHnw@2x.png)也就是某種的交換律

用上面那邊文章的圖做解釋
  **pk** ：私鑰
  **P**  ：公鑰
  **H(m)** ：可以看作是hash過的message
  **S** ：簽章

驗證簽章會滿足
e(P, H(m)) = e(G, S)

也就是 **signature** 可以用P（公鑰）跟 H(m)（hash過的message）做驗證，跟我們以往的認知是一致的。從公式看BLS在sign跟verify都很簡潔，資料量的部分也小了許多（好像是33 bytes）。而ECDSA在verify的部分就複雜了一點（需要先算出v值），細節可以參考[這裡](http://kimiwublog.blogspot.com/2018/06/ecdsaethereumsign-message.html)。簽章的加總（signature aggregation）簡單來講，就是利用上面提到的交換律所達成，細節可以參考上面提到的文章，這裡就不多提了。

#### 省了空間，那效能呢？！

如果有把BLS signatures: better than Schnorr看過，最下面會提到，看起來很美好，其實很不實用，因為要找尋特殊的對稱曲線，其實很困難及複雜，所以在verify時會比原本的ECDSA更久。（啥？！ 那Casper幹嘛用它！！）實際上Ethereum用[BLS128-381](https://blog.z.cash/new-snark-curve/)，是去年Zcash發表的，是非對稱的橢圓曲線，針對128bits的應用上做了最佳化，所以也解決了效能上的問題。

根據Justin Drake提供的數據，2/3validators(預估總共validator數量為 312,500)的簽章大約會是40K，verify速度大約在300ms左右，但是離線蒐集跟打包signature大約要9分鐘，所以每次finality大約可以在10分鐘左右完成

最後！這個是Ethereum中期的簽章方案，長期的預計會使用zk-STARK，zk-STARK的設計是可以抗量子攻擊，但目前資料量約在100kB左右，還會針對Ethereum做最佳化。

附：這有[Ethereum meeting 討論BLS的影片](https://www.youtube.com/watch?v=DpV0Hh9YajU&index=5&list=PLaM7G4Llrb7zEHK2UzQo3kxadPyeUy2sZ)
