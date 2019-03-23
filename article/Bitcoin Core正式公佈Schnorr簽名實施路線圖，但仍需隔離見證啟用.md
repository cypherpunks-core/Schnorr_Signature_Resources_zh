# Bitcoin Core正式公佈Schnorr簽名實施路線圖，但仍需隔離見證啟用

[kyle ](https://www.8btc.com/author/14244)2017-03-24 10:20釋出在[ 比特幣 ](javascript:;) 19906

Bitcoin Core開發者今日公佈了[新的技術發展路線圖](https://bitcoincore.org/en/2017/03/23/schnorr-signature-aggregation/)，計劃將目前的數字簽名演算法過渡到一種更加先進的替代性選擇。

![hcm-roadmap-940x460|766x460](https://cdn.8btc.com/wp-content/uploads/2017/03/hcm-roadmap-940x460.jpg)

如果獲得實施，該[提案](https://bitcoincore.org/en/2017/03/23/schnorr-signature-aggregation/)將會使用“Schnorr簽名“替代比特幣目前所使用的”ECDSA簽名”為交易進行簽名。通過實施這種切換，開發者認為他們可以 **使比特幣區塊鏈的總資料量降低高達25%** 。

對於使用者而言，這意味著儲存網路交易歷史的節點將擁有更好的頻寬，同時使用更少的儲存來保護整個區塊鏈的安全。

根據這個路線圖的描述：

> “假設每個歷史簽名都降低到1位元組，分析顯示這種方法將使所需要的儲存和頻寬降低至少25%。”
在去年10月份的米蘭擴容會議上，比特幣的開源開發團隊向比特幣發展路線圖引入了更改簽名的計劃。

當時，Bitcoin Core開發者Pieter Wuille為宣傳這個計劃進行了慷慨激昂的講話，同時呼籲更廣泛的社群來幫助解決一些障礙。

要想實施Schnorr簽名，比特幣網路將需要對其 `OP_CHECKSIG and OP_CHECKMULTISIG` 函數進行一些修改，從而使開發者可以堆疊公鑰。

目前為止，比特幣整個區塊鏈的體積已經達到大約[110GB](https://blockchain.info/charts/blocks-size)。

 

## 保留意見

然而，這種更改簽名演算法的想法並不非暢通無阻。

根據Wuille所說，Schnorr簽名面臨著一種“作廢（cancellation）“問題，這個問題可能會對使那些具有敵意的參與者有機會減去一個來自多重簽名交易的金鑰以及移除錢包中的一位參與者。

此外，Core開發者Greg Maxwell表示整合Schnorr並不需要啟用隔離見證（SegWit），不過他也表示如果使用隔離見證，那麼整合過程會更簡單一些。

為此，在SegWit啟用正式確定下來之前，Schnorr簽名的功能不可能被實施。

Maxwell說：

> “我對在沒有隔離見證的情況下實施Schnorr感到懷疑，儘管有可能。
如今比特幣擴容問題的進展幾乎已經陷入停滯和分歧之中，[比特幣開發者已經決定在今年5月份召開一次會議](http://www.8btc.com/scaling-meeting-take-place-may)，試圖能夠團結行業參與者，共同解決擴容問題。