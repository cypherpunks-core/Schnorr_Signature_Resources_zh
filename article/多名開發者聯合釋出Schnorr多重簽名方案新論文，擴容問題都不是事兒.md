# 多名開發者聯合釋出Schnorr多重簽名方案新論文，擴容問題都不是事兒
來源：https://www.8btc.com/author/14244
[kyle ](https://www.8btc.com/author/14244)2018-01-19 11:32釋出在[ 比特幣 ](javascript:;) 13721

一份新的針對Schnorr多重簽名的研究論文剛剛釋出——《[Schnorr多重簽名在比特幣的應用](http://8btc.com/doc-view.html?d=1759)》（[幣文庫下載](http://8btc.com/doc-view.html?d=1759)），由多位著名的比特幣開發者親自撰寫。

[![QQ截圖20180119112129|708x425](https://cdn.8btc.com/wp-content/uploads/2018/01/201801190322115358.jpg)](https://cdn.8btc.com/wp-content/uploads/2018/01/201801190322115358.jpg)

這份論文釋出於本週四，作者包括開發者Gregory Maxwell, Andrew Poelstra, Yannick Seurin 和Pieter Wuille。論文詳細介紹了Schnorr多重簽名如何能夠應用於比特幣，雖然不能保證最終都會被使用，但這個新發布可能標誌著朝著這個方向邁出的又一步。

具體而言，Schnorr概念提出將多個簽名捆綁到一個小的資料條目中，而不是單獨列出多個簽名。這份論文認為，此舉將節省區塊鏈上的空間，使區塊鏈能夠處理更多的簽名，同時增加安全性。

安全性可通過啟用多重簽名系統來增加，這個過程至少需要交易獲得兩個確認。這將限制或阻止惡意分子利用自己的另一個使用者帳戶來啟動交易。

論文作者寫道：

> “在這種情況下，多重簽名的大小與簽名者的數量成線性關係。為了能夠發揮用途，一個多重簽名方案應該能夠生成大小(理想情況下)與簽名者的數量無關的簽名，並且這種簽名的大小要接近普通簽名方案。"
> 如果實現的話，Schnorr簽名也可以提供額外的好處。

將資料與一個簽名進行捆綁能夠限制區塊鏈上的垃圾郵件。換句話說，取代將許多小的資料區塊傳送到網路，而是打包成一個再發送，這樣可以更快地處理這些資料。

同樣，將不同來源的資料打包在一起能夠提高隱私性，因為這樣更加難以跟蹤某一筆交易的來源。

《[比特幣擴容如何解決？Schnorr簽名可能成為比特幣的下一步](http://www.8btc.com/schnorr-signatures-might-be-bitcoins-next-step-forward)》

《[Schnorr簽名將解決比特幣的兩個最大問題：擴充套件性和垃圾交易攻擊](http://www.8btc.com/schnorr-signatures-2-of-bitcoins-biggest-problems)》

《[Bitcoin Core正式公佈Schnorr簽名實施路線圖，但仍需隔離見證啟用](http://www.8btc.com/bitcoin-core-schnorr-signature)》
