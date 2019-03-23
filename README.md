# Schnorr簽名資源 | Schnorr Signature Resources

![](https://img.shields.io/badge/Powered%20by-Chen%20Po%20Wei-blue.svg)
![](image.png)

-   [Bitcoin Q&A: Schnorr signatures and the privacy roadmap](https://www.youtube.com/watch?v=JeJzwZgxF50)-aantonop

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

-   [Hash function requirements for Schnorr signatures](paper/Hash-Function-Requirements-for-Schnorr-Signatures.pdf)
    We provide two necessary conditions on hash functions for the Schnorr signature scheme to be secure, assuming compact group representations such as those which occur in elliptic curve groups. We also show, via an argument in the generic group model, that these conditions are sufficient. Our hash function security requirements are variants of the standard notions of preimage and second preimage resistance. One of them is in fact equivalent to the Nostradamus attack by Kelsey and Kohno (Eurocrypt 2006), and, when considering keyed compression functions, both are closely related to the ePre and eSec notions by Rogaway and Shrimpton (FSE 2004).
    Our results have a number of interesting implications in practice. First, since security does not rely on the hash function being collision resistant, Schnorr signatures can still be securely instantiated with SHA-1/SHA-256, unlike DSA signatures. Second, we conjecture that our properties require O(2n) work to solve for a hash function with n-bit output, thereby allowing the use of shorter hashes and saving twenty-five percent in signature size. And third, our analysis does not reveal any significant difference in hardness between forging signatures and computing discrete logarithms, which plays down the importance of the loose reductions in existing random-oracle proofs, and seems to support the use of “normal-size” groups.

-   [Efficient Identification and Signatures for Smart Cards](http://sci-hub.tw/https://link.springer.com/chapter/10.1007%2F0-387-34805-0_22)
    We present an efficient interactive identification scheme and a related signature scheme that are based on discrete logarithms and which are particularly suited for smart cards. Previous cryptoschemes, based on the discrete logarithm, have been proposed by El Gamal (1985), Chaum, Evertse, Graaf (1988), Beth (1988) and Günter (1989). The new scheme comprises the following novel features.


-   [How To Prove Yourself: Practical Solutions to Identification and Signature Problems](http://sci-hub.tw/https://link.springer.com/chapter/10.1007%2F3-540-47721-7_12)  
    In this paper we describe simple identification and signature schemes which enable any user to prove his identity and the authenticity of his messages to any other user without shared or public keys. The schemes are provably secure against any known or chosen message attack if factoring is difficult, and typical implementations require only 1% to 4% of the number of modular multiplications required by the RSA scheme. Due to their simplicity, security and speed, these schemes are ideally suited for microprocessor-based devices such as smart cards, personal computers, and remote control systems.


-   [Attacks on Schnorr signatures with biased nonces](https://ecc2017.cs.ru.nl/slides/ecc2017-tibouchi.pdf)
-   [On the Exact Security of Schnorr-Type Signatures in the Random Oracle Model](https://eprint.iacr.org/2012/029.pdf)
    The Schnorr signature scheme has been known to be provably secure in the Random Oracle Model under the Discrete Logarithm (DL) assumption since the work of Pointcheval and Stern (EUROCRYPT ’96), at the price of a very loose reduction though: if there is a forger making at most  _q_   _h_  random oracle queries, and forging signatures with probability  _ε_   _F_  , then the Forking Lemma tells that one can compute discrete logarithms with constant probability by rewinding the forger (𝑞ℎ/𝜀𝐹)O(qh/εF) times. In other words, the security reduction loses a factor (𝑞ℎ)O(qh) in its time-to-success ratio. This is rather unsatisfactory since  _q_   _h_  may be quite large. Yet Paillier and Vergnaud (ASIACRYPT 2005) later showed that under the One More Discrete Logarithm (OMDL) assumption, any  _algebraic_  reduction must lose a factor at least 𝑞1/2ℎqh1/2 in its time-to-success ratio. This was later improved by Garg  _et al._  (CRYPTO 2008) to a factor 𝑞2/3ℎqh2/3. Up to now, the gap between 𝑞2/3ℎqh2/3 and  _q_   _h_  remained open. In this paper, we show that the security proof using the Forking Lemma is essentially the best possible. Namely, under the OMDL assumption, any algebraic reduction must lose a factor  _f_ ( _ε_   _F_  ) _q_   _h_  in its time-to-success ratio, where  _f_  ≤ 1 is a function that remains close to 1 as long as  _ε_   _F_  is noticeably smaller than 1. Using a formulation in terms of expected-time and queries algorithms, we obtain an optimal loss factor Ω( _q_   _h_  ), independently of  _ε_   _F_  . These results apply to other signature schemes based on one-way group homomorphisms, such as the Guillou-Quisquater signature scheme.


-   [Schnorr Non-interactive Zero-Knowledge Proof](https://www.rfc-editor.org/rfc/pdfrfc/rfc8235.txt.pdf)
    This document describes the Schnorr non-interactive zero-knowledge (NIZK) proof, a non-interactive variant of the three-pass Schnorr identification scheme. The Schnorr NIZK proof allows one to prove
    the knowledge of a discrete logarithm without leaking any information about its value. It can serve as a useful building block for many cryptographic protocols to ensure that participants follow the
    protocol specification honestly. This document specifies the Schnorr NIZK proof in both the finite field and the elliptic curve settings.
