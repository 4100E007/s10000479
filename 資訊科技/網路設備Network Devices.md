# 網路設備Network Devices
![image](https://user-images.githubusercontent.com/90738394/138015854-b2fe071c-cdf2-4a18-8430-50c8e04b68eb.png)
# [OSI](https://ithelp.ithome.com.tw/articles/10234845)
> Open System Interconnection（OSI）是七層的網路架構，稱為開放式系統互聯參考模型，是一個抽象、理論的模型，它將網路分為七層的主要目的是為了解決異構網路互連時所遇到的兼容性問題。最大的優點是將service、port和protocol這三個概念明確區分開來，通過七個層次的結構模型使不同的系統和不同的網路之間實現可靠的通訊。
## 第一層實體層 [physical layer](https://zh.wikipedia.org/wiki/%E7%89%A9%E7%90%86%E5%B1%82)
> 提供雙方系統間實體介面、傳送位元的規則。控制電腦介面如何經由網路來交談，這一層指定了電子規格。傳輸介質的規格、接頭的規格、資料在介質上的呈現方式
### [repeater 中繼器](https://zh.wikipedia.org/wiki/%E4%B8%AD%E7%BB%A7%E5%99%A8)
- 一個將輸入訊號增強放大的類比裝置(以防中途中斷)，而不考慮輸入訊號種類（是類比的還是數位的）。中繼器是用來加強纜線上的訊號，把訊號送得更遠，以延展網路長度
### [hub 集線器](https://zh.wikipedia.org/wiki/%E9%9B%86%E7%B7%9A%E5%99%A8)
-集線器是運作在OSI模型中的實體層[1]，可以讓其連結的裝置工作在同一網段。
-由於集線器會把收到的任何數位訊號，經過再生或放大，再從集線器的所有埠送出，這會造成訊號之間碰撞的機會很大，而且訊號也可能被竊聽，並且這代表所有連到集線器的裝置，都是屬於同一個碰撞網域以及廣播網域，因此大部份集線器已被交換機取代。
- 集線器的種類 被動型集線器（Passive Hub），集線器不需連接電源，因此網路訊號隨距離衰減，只適用於短距離的網路連接。
主動型集線器（Active Hub），集線器需連接電源，可加強訊號強度（整波放大）。

## 第二層資料連結層 [data link layer](https://zh.wikipedia.org/wiki/%E6%95%B0%E6%8D%AE%E9%93%BE%E8%B7%AF%E5%B1%82)
> 提供Network Layer及Physical Layer間之管理、錯誤偵測與控制。將要送經網路的資料包裝及拆裝，組織這些位元。負責將資料切割成真正的資料框，並將之送至傳輸媒介上。其中常見的封包碰撞機制：CSMA/CA和CSMA/CD。分為兩個子層：邏輯鏈路控制（logical link control，LLC）子層和媒介存取控制（Media access control，MAC）子層。
### 交換器(switch)
- 通過報文交換接收和轉發資料到目標裝置，它能夠在電腦網路上連接不同的裝置。
- 交換器是一種多埠的網橋，在資料鏈路層使用`MAC位址`轉發資料。
- 交換器內部的CPU會在每個埠成功連接時，通過將MAC位址和埠對應，形成一張MAC表。在今後的通訊中，發往該MAC位址的封包將僅送往其對應的埠，而不是所有的埠
- 當一台交換器安裝組態好之後，其工作過程如下：
   -收到某網段（設為A）MAC位址為X的電腦發給MAC位址為Y的電腦的封包。交換器從而記下了MAC位址X在網段A。這稱為學習（learning）。
   -交換器還不知道MAC位址Y在哪個網段上，於是向除了A以外的所有網段轉發該封包。這稱為泛洪（flooding）。
   -MAC位址Y的電腦收到該封包，向MAC位址X發出確認包。交換器收到該包後，從而記錄下MAC位址Y所在的網段。
   -交換器向MAC位址X轉發確認包。這稱為轉發（forwarding）。
   -交換器收到一個封包，查表後發現該封包的來源位址與目的位址屬於同一網段。交換器將不處理該封包。這稱為過濾（filtering）。
   -交換器內部的MAC位址-網段查詢表的每條記錄採用時間戳記錄最後一次存取的時間。早於某個閾值（使用者可組態）的記錄被清除。這稱為老化（aging）。
   -對於全交換（full-switch）區域網路，交換器每個埠只連接一台裝置，因此不會發生碰撞。交換器也不需要做過濾。

## 第三層網路層 
> 提供雙方透過網路的定址方法、傳送路徑。在點對點傳輸中，由於Data Link Layer已提供管理之功能，因此用不到此層。指定使用者資料轉送至網路的界面，負責資料的包封及傳輸途徑的設定。
### [router 路由器](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E5%99%A8)
- 提供路由與轉送兩種重要機制，可以決定封包從來源端到目的端所經過的路徑（host到host之間的傳輸路徑）
- 路由器是提供 Wi-Fi 的裝置，可將互聯網的資訊傳送至個人裝置 (例如電腦、手機或平板電腦)。這些連接互聯網的裝置在您家中會形成局部區域網絡 (LAN)。
- 路由器就是連接兩個以上個別網路的裝置。
- 路由工作在OSI模型的第三層——即網路層，例如網際協定（IP）
- 路由器與交換機的差別，路由器是屬於OSI第三層的產品，交換器是OSI第二層的產品。

[路由器參考](https://24h.pchome.com.tw/prod/DRAN36-A900AV1WC)
## 第四層傳輸層
> 傳輸層（Transport Layer）把傳輸表頭（TH）加至數據以形成數據包。傳輸表頭包含了所使用的協定等傳送資訊。例如:傳輸控制協定（TCP）等。
## 第五層會議層
> 會議層（Session Layer）負責在數據傳輸中設定和維護電腦網路中兩台電腦之間的通訊連接。
## 第六層表達層
> 表達層（Presentation Layer）把數據轉換為能與接收者的系統格式相容並適合傳輸的格式。
## 第七層應用層
> 應用層（Application Layer）提供為應用軟體而設計的介面，以設定與另一應用軟體之間的通訊。例如：HTTP、HTTPS、FTP、Telnet、SSH、SMTP、POP3等。


![image](https://user-images.githubusercontent.com/90738394/138378076-ca9d499b-937b-4bf5-b10b-658b94329f2d.png)

## Transmission Control Protocol / Internet Protocol（TCP/IP）是目前使用最廣泛的網路協定，相較於OSI模型將網路功能分成七層，TCP/IP模型則是將網路功能分成四層，但它並不是將OSI模型中的某些層去掉，而是將功能類似的層合併。
### Link Layer
> 這一層又稱網路介面層（Network Interface Layer），負責與硬體溝通，雖然沒有定義任何通訊協定，但基本上，它支援所有標準的通訊協定。
### Network Layer
> 這一層又稱網際網路層（Internet Layer），負責定址與路由等工作，而且資料是以資料元（datagram）為單位，比較知名的通訊協定有IP（Internet Protocol）。
### Transport Layer
> 這一層又稱主機對主機層（Host-to-Host Layer），負責區段排序、錯誤控制、流量控制等工作，比較知名的通訊協定有TCP（Transmission Control Protocol）、UDP（User Datagram Protocol）。
### Application Layer
> 這一層負責提供網路服務給應用程式，比較知名的通訊協定有FTP（File Transfer Protocol, 檔案傳輸協定）、SMTP（Simple Mail Transfer Protocol, 簡易郵件傳送協定）、POP（Post Office Protocol, 郵件接收協定）、DNS（Domain Name System, 網域名稱系統）、Telnet（遠端登入）、SNMP（Simple Network Management Protocol, 簡易網路管理協定）、HTTP（HyperText Transfer Protocol, 超文字傳輸協定）、NNTP（Network News Transfer Protocol）…等。

## 通訊協定
> 通信協定（英語：Communications Protocol，也稱傳輸協定）在電信領域中指的是，在任何物理媒介中允許兩個或多個在傳輸系統中的終端之間傳播資訊的系統標準，也是指電腦通信或網路裝置的共同語言。[1]， 通信協定定義了通信中的語法學、語意學和同步規則以及可能存在的錯誤檢測與糾正。通信協定在硬體、軟體或兩者之間皆可實現[2]
> 

