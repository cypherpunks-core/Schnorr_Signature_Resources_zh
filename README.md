# Schnorr簽名資源 | Schnorr Signature Resources

![](image.png)

## Medium

-   [Ethereum Casper - 認識 BLS signature](article/EthereumCasper-認識BLSsignature.md)

## Ethfans

-   [比特幣下一次升級要包含的Taproot究竟是什麼](article/比特幣下一次升級要包含的Taproot究竟是什麼.md)

## 8btc

-   [Schnorr簽名的前世今生：為什麼說比特幣的隱私性是不可避免的？](article/Schnorr簽名的前世今生：為什麼說比特幣的隱私性是不可避免的？.md)
-   [MuSig : 比特幣可用的Schnorr簽名方案](article/MuSig:比特幣可用的Schnorr簽名方案.md)
-   [比特幣再迎重大技術突破，Schnorr簽名程式碼正式開放測試](article/比特幣再迎重大技術突破，Schnorr簽名程式碼正式開放測試.md)
-   [學術向丨Schnorr簽名方案和BLS簽名方案的全面對比](article/學術向丨Schnorr簽名方案和BLS簽名方案的全面對比.md)
-   [區塊鏈替代簽名方案優劣勢對比，Schnorr簽名最適合比特幣](article/區塊鏈替代簽名方案優劣勢對比，Schnorr簽名最適合比特幣.md)
-   [隔離見證（SegWit）之後，比特幣有望迎來最重磅升級——Schnorr](article/隔離見證（SegWit）之後，比特幣有望迎來最重磅升級——Schnorr.md)
-   [提升交易速度，降低手續費，Schnorr簽名即將成為比特幣的重要技術](article/提升交易速度，降低手續費，Schnorr簽名即將成為比特幣的重要技術.md)
-   [多名開發者聯合釋出Schnorr多重簽名方案新論文，擴容問題都不是事兒](article/多名開發者聯合釋出Schnorr多重簽名方案新論文，擴容問題都不是事兒.md)
-   [Schnorr簽名將解決比特幣的兩個最大問題：擴充套件性和垃圾交易攻擊](article/Schnorr簽名將解決比特幣的兩個最大問題：擴充套件性和垃圾交易攻擊.md)
-   [Bitcoin Core正式公佈Schnorr簽名實施路線圖，但仍需隔離見證啟用](article/BitcoinCore正式公佈Schnorr簽名實施路線圖，但仍需隔離見證啟用.md)
-   [Schnorr簽名的威力：強化比特幣可擴充套件性和隱私的簽名演算法](article/Schnorr簽名的威力：強化比特幣可擴充套件性和隱私的簽名演算法.md)

## 論文

-   [可防止提權攻擊之階層式安全比特幣錢包機制](https://hdl.handle.net/11296/kuku5v)：隨著比特幣日益普及，人們傾向於使用比特幣錢包來管理用來支出或接受資金的金鑰。階層式確定性(HD)錢包不是隨機生成不便於存儲的金鑰對，而是從單一種子來派生所有金鑰，因此只要存儲該種子便足以恢復金鑰。HD錢包中允許使用者在不知道任何私鑰的情況下從父公鑰生成子公鑰，這個功能的一個合適情況是允許稽查人員導出所有公鑰以進行審計的案例。然而，這個優秀的特性卻使得HD錢包遭受到所謂的提權攻擊，意即任意一個子私鑰和主公鑰的洩漏就會導致整個錢包中的所有密鑰洩漏出去。為了應對這個嚴重的問題，我們提出了一種新的HD錢包機制，該機制使用陷門雜湊函數發出簽章，而不是直接提供給任何人私鑰以產生簽章，因此可以防止提權攻擊的發生。然而，我們所提出的方案提供了兩個公鑰之間的不可連結性，以實現用戶身分的匿名性和金鑰派生的高可擴展性。因此，我們的機制實現了匿名性、公鑰派生以及高可擴展性。
