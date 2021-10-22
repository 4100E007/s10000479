# 網路設備Network Devices
![image](https://user-images.githubusercontent.com/90738394/138015854-b2fe071c-cdf2-4a18-8430-50c8e04b68eb.png)
# OSI
## 第一層實體層 [physical layer](https://zh.wikipedia.org/wiki/%E7%89%A9%E7%90%86%E5%B1%82)
### [repeater 中繼器](https://zh.wikipedia.org/wiki/%E4%B8%AD%E7%BB%A7%E5%99%A8)
- 一個將輸入訊號增強放大的類比裝置(以防中途中斷)，而不考慮輸入訊號種類（是類比的還是數位的）。中繼器是用來加強纜線上的訊號，把訊號送得更遠，以延展網路長度
### [hub 集線器](https://zh.wikipedia.org/wiki/%E9%9B%86%E7%B7%9A%E5%99%A8)
-集線器是運作在OSI模型中的實體層[1]，可以讓其連結的裝置工作在同一網段。
-由於集線器會把收到的任何數位訊號，經過再生或放大，再從集線器的所有埠送出，這會造成訊號之間碰撞的機會很大，而且訊號也可能被竊聽，並且這代表所有連到集線器的裝置，都是屬於同一個碰撞網域以及廣播網域，因此大部份集線器已被交換機取代。
- 集線器的種類 被動型集線器（Passive Hub），集線器不需連接電源，因此網路訊號隨距離衰減，只適用於短距離的網路連接。
主動型集線器（Active Hub），集線器需連接電源，可加強訊號強度（整波放大）。

## 第二層資料連結層 [data link layer](https://zh.wikipedia.org/wiki/%E6%95%B0%E6%8D%AE%E9%93%BE%E8%B7%AF%E5%B1%82)
### 交換器(switch)
- 通過報文交換接收和轉發資料到目標裝置，它能夠在電腦網路上連接不同的裝置。
- 交換器是一種多埠的網橋，在資料鏈路層使用`MAC位址`轉發資料。
- 交換器內部的CPU會在每個埠成功連接時，通過將MAC位址和埠對應，形成一張MAC表。在今後的通訊中，發往該MAC位址的封包將僅送往其對應的埠，而不是所有的埠


## 第三層網路層 
### [router 路由器](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E5%99%A8)
- 提供路由與轉送兩種重要機制，可以決定封包從來源端到目的端所經過的路徑（host到host之間的傳輸路徑）
- 路由器是提供 Wi-Fi 的裝置，可將互聯網的資訊傳送至個人裝置 (例如電腦、手機或平板電腦)。這些連接互聯網的裝置在您家中會形成局部區域網絡 (LAN)。
- 路由器就是連接兩個以上個別網路的裝置。
- 路由工作在OSI模型的第三層——即網路層，例如網際協定（IP）
- 路由器與交換機的差別，路由器是屬於OSI第三層的產品，交換器是OSI第二層的產品。

[路由器參考](https://24h.pchome.com.tw/prod/DRAN36-A900AV1WC)


![image](https://user-images.githubusercontent.com/90738394/138378076-ca9d499b-937b-4bf5-b10b-658b94329f2d.png)


