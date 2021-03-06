# 提升交易速度，降低手續費，Schnorr簽名即將成為比特幣的重要技術
來源：https://www.8btc.com/author/40583
[Captain Hiro ](https://www.8btc.com/author/40583)2018-02-13 16:37釋出在[ 比特幣 ](javascript:;) 11066

> “To the moon！”
> 當一個幣種開始爬升時，這一加密貨幣的口號就會經常被使用，而這一次，這一口號被用作表達人們對於長期等待的比特幣編碼優化程式的激動之情。

被稱作Schnorr簽名，這一技術將取代比特幣現有的簽名。這一概念之所以很吸引人，有一部分原因是它可以清理區塊鏈上的空間，這樣可以幫助解決比特幣使用者經常需要面對的交易延遲以及高手續費的問題。

[![Schnorr簽名|750x450](https://cdn.8btc.com/wp-content/uploads/2018/02/201802130834021281.jpg)](https://cdn.8btc.com/wp-content/uploads/2018/02/201802130834021281.jpg)

根據正在開發這項技術的開發者所述，這一改變將會導致比特幣的交易容量增大25%到30%。

Yannick Seurin是一個法國網路安全機構ANSSI的密碼破譯高手，他正在研究Schnorr背後的這一密碼系統，並告訴Coindesk：

> “Schnorr簽名以及應用可以產生非常高的期待值。從擴容爭論中可以看出，任何可以提高效率的改進對比特幣都是大有好處的。”
> 的確，比特幣社群正在團結一致，圍繞著幾個技術來讓比特幣支付的使用更有效率、更便宜、更快速並更簡便。Schnorr只是很多技術中的一個，其他的還有聯合的FIBRE網路，點對點的優化，以及最有野心的項目，馬上要到來的閃電網路。

但是Schnorr最近卻成為了一些知名的比特幣開發者所關注的焦點。

這不僅僅是因為隔離見證（Segwit）最終在比特幣上被啟用，同時還因為Schnorr簽名能提供其他的好處，比如提高特定交易形式的隱私性，以及減少那些堵塞網路的垃圾交易。

舉個例子，Jonas Nick對CoinDesk說，他對於其隱私方面的優勢更感興趣，這對於Blockstream的基礎設施安全工程師來說並不奇怪。同樣，他同時也關注於如何可以親手改變其他的程式碼，從而可以解鎖更多現金的比特幣使用案例。

> “事實上，我對於這種工作感到非常興奮，它的目標就像智慧合約在鏈上看起來像普通的支付一樣。Schnorr簽名起到了一個至關重要的作用，還有MAST、Taproot以及Graftroot。”Nick說道，並提到了在促進比特幣智慧合約的發展過程中一系列的改變。

## 巧妙的攻擊

關於Schnorr的這份激動已經等待了很長時間了——這一技術是從2012年開始開發的。

儘管這看起來對於一些人很好奇，但是對於那些和技術接觸比較多的人來說，這些拖延並不讓人感到吃驚。首先，並沒有那麼多的瞭解比特幣以及密碼學的開發者可以幫助來改變像是Schnorr這樣的項目。

其次，自從Schnorr將要成為一個價值1000億美元的比特幣網路上的重大改變，那麼這一技術就需要大量的同行審查和測試。

這兩點確實減慢了Schnorr的進展。

根據知名的比特幣貢獻者，同時也是Blockstream的共同建立人Pieter Wuille在斯坦福的演講所述，Schnorr在過去的幾年中經歷了幾個“不容易被發現的挑戰”。

比如說，在去年Wuille以及其它開發者在Schnorr實施時發現了一個“流氓攻擊”，使他們呈遞了一篇文章勾勒出了可能要進行的修訂。但是學會駁回了遞交的文章，並指出了一篇更好的文章——雖然這和比特幣沒有關係，但是者卻強調了這一攻擊載體使用了更安全的方式。

這就是ANSSI密碼專家Seurin加入比特幣開發者的原因。

> “我注意到他們考慮的具體簽名融合方案並沒有一個基於實踐的合理安全分析，”他說道。“而安全證明是我專門的研究領域，同時我先前工作於Schnorr簽名的項目，我就聯絡了Pieter Wuille。”
> Wuille隨後給Seurin發了一篇文章，同時和Bitcoin Core的貢獻者Gregory Maxwell 以及Blockstream的數學家Andrew Pwolstra一同寫了一個更安全的構造。

儘管這一構造起到了一定的作用，但是另一個問題卻在隨後湧現出來。

另一個攻擊載體被Blockstream的工程師Russell O’Connor發現（Wuille將其稱作“Russell’s attack”），這一問題可以使得使用者偷取使用簽名交易的比特幣。

在演講中，Wuille說道：

> “從中能學到的，至少對於我自己來說，就是多方策劃的攻擊模型可以非常巧妙。這並不是那麼顯而易見的。”

## 過程和謹慎觀點

這些攻擊載體被解決了，但是這一技術的工作還將持續。

現在有幾個比特幣改進建議（BIPs）正在起著作用，Wuille高速參加演講的觀眾。同時一旦這些完成了，它將提供新的簽名計劃是如何工作的，以及它是如何被新增到比特幣上去的。再加上其他的比特幣貢獻者們將會有機會對於這一項目的實施進行審查，並提出改變的建議。

更不用說，一個程式碼的實施需要在發展過程中需要很長的時間，Nick說很多時候進行的是模糊測試。模糊測試是隨機投擲一段程式碼中的資料，並檢查是否回來的輸出總是正確的。

> “當你在大量的事件中用很多的程式碼來進行每秒鐘上百次的測試，模糊測試是歷史上找到微妙漏洞的一個很好的追蹤記錄，”Nick對CoinDesk說道，並補充道：“我們沒有發現問題……這增強了我們在實施過程中的信心。”
> 根據Wuille所述，如果上述情況持續下去的話，Schnorr程式碼的完成不會花很長的時間。

在談話中，Wuille說道，“忽視謹慎觀點，通過隔離見證的指令碼版本化來增添opcode並不是很難的一件事。”

然而，隨著圍繞著隔離見證啟用的爭論，謹慎的觀點也許會成為一件很難忽視的事情。

任何一種方法，程式碼的改變在最近都吸引了很多的關注，開發者也一直在寫博文，同時有很多人也在Reddit上進行討論。

但是由於在線上有著數千億美元，如果一次升級擾亂了比特幣執行的方式，那麼絕大多數的持有者也許對於很快的增加程式碼這件事感到猶豫。

Bitcoin Core的貢獻者Nicolas Dorier估計Schnorr要增添到比特幣上可能要花去很多年的時間。

甚至是Wuille在演講過程中，也承認這一時間線的必要性。

> 他總結道：“我非常期待看到我們一直工作的這個項目融合到比特幣上會是什麼樣，但是這是一個漫長的過程。”
