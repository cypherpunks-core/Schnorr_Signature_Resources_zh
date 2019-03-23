# 彌補中本聰的遺憾！Schnorr簽名有望在2020年在比特幣上正式實現

[kyle ](https://www.8btc.com/author/14244)2019-03-19 11:08釋出在[ 比特幣 ](javascript:;)[獨家 ](javascript:;) 56659

比特幣開發者、密碼學家、Blockstream研究主管安德魯·波爾斯特拉(Andrew Poelstra)表示，“未來幾周”可能會將一份正式的比特幣[Schnorr簽名](https://www.8btc.com/article/374308)升級提案提交給比特幣開發者郵件列表。Poelstra補充說，比特幣網路可能會在2020年實現Schnorr簽名。這些聲明是幾天前他在彼得·麥考馬克(Peter McCormack)主持的“What Bitcoin Did播客上發表的。

[![QQ截圖20190319104442\_副本|984x590](https://cdn.8btc.com/wp-content/uploads/2019/03/201903190245431003.jpg)](https://cdn.8btc.com/wp-content/uploads/2019/03/201903190245431003.jpg)

圖片來源：[pexels](https://www.pexels.com/photo/office-working-app-computer-97077/)

> “我希望在接下來的幾周內，我們能最終寫下一份提案，並提交到比特幣郵件列表中。我們在這個叫做sigcash no input的東西上來回思考了很多次，不幸的是，這和其他東西沒有太多相關。”

## ECDSA和Schnorr

Schnorr簽名是一件大事，它可以顯著提高比特幣網路的隱私性和空間效率，甚至不需要硬分叉就能在比特幣網路上實施。比特幣目前主要使用Schnorr簽名的一個變通版本來滿足其簽名需求，稱為橢圓曲線數字簽名演算法(ECDSA)。

ECDSA是作為一種標準化的、開源的替代方案開發的，而不是更簡單、公認更好的Schnorr簽名。ECDSA的解決方案是必要的，因為Schnorr簽名的發明者Claus Schnorr在80年代為他的發明申請了專利——據Poelstra說，密碼學標準機構並不願接受這種情況。

Schnorr簽名的專利於2008年到期，當時比特幣發明人中本聰正在開發比特幣。儘管後來Schnorr可以免費使用，但並沒有得到廣泛的支援。因此，中本聰選擇ECDSA作為比特幣的標準簽名方案。

Schnorr簽名可以將任意數量的交易和/或私鑰持有者“聚合”到單個簽名的儲存空間中。這可以節省節點和礦工在一個區塊中驗證每個單獨簽名的時間。更重要的是，它允許被聚合和多簽名的交易看起來與其他所有交易一樣——這意味著單個、多簽名的、甚至閃電網路交易看起來都是相同的。

這是因為比特幣目前的多簽名機制，即更為繁瑣的Pay-to-ScriptHash (P2SH)，需要一種特殊的地址格式，這種格式對於區塊鏈觀測器而言就像一個巨大的訊號旗，能夠輕易被分辨出來，表明某筆多重簽名交易已經完成。不過，Schnorr下的簽名聚合將使此類交易實際上不可見。

## Schnorr簽名技術準備就緒

在播客中，同時也是Grin隱私幣主要開發者之一的Poelstra表示，Blockstream“幾乎已經為Bitoin Core編寫好了(Schnorr)程式碼”。事實上，Schnorr簽名升級的草案已經在[網上](https://github.com/sipa/bips/blob/bip-schnorr/bip-schnorr.mediawiki)公佈了。

他說，這段程式碼將被納入下一個Bitcoin Core版本（不被啟用）中，並在“討論……實際的啟用參數”之後獲得批准，然後正式啟用。
