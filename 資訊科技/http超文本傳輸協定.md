## http
[HyperText Transfer Protocol](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol)

[超文本傳輸協議](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE)
- 超文本傳輸協定（英語：HyperText Transfer Protocol，縮寫：HTTP）是一種用於分佈式、協作式和超媒體訊息系統的```應用層```協定
![image](https://user-images.githubusercontent.com/90738394/138025018-0da92489-cb04-4536-ba37-462f5d94a33c.png)
## http request
---
![image](https://user-images.githubusercontent.com/90738394/138025167-1ad6bd2a-4cc4-4b52-9a56-3e6039dcae97.png)


## http response
![image](https://user-images.githubusercontent.com/90738394/138025288-20fe6168-2144-4353-88cc-f94f0448bb15.png)

## HTTP狀態碼
| 狀態碼 | 類型 |
| ------ | ------ |
|1xx訊息|代表請求已被接受，需要繼續處理|
|2xx成功|代表請求已成功被伺服器接收、理解、並接受|
|3xx重新導向|需要客戶端採取進一步的操作才能完成請求。通常，這些狀態碼用來重新導向|
|4xx客戶端錯誤|客戶端可能發生了錯誤，妨礙了伺服器的處理。|
|5xx伺服器錯誤|伺服器無法完成明顯有效的請求。[56]這類狀態碼代表了伺服器在處理請求的過程中有錯誤或者異常狀態發生|
### 請求方法
> http中定義了8種方法

| 方法 | 說明 |
| ------ | ------ |
| GET | 向指定的資源發出「顯示」請求。使用GET方法應該只用在讀取資料 |
| HEAD | 與GET方法一樣，都是向伺服器發出指定資源的請求。只不過伺服器將不傳回資源的本文部份 |
| POST | 向指定資源提交資料，請求伺服器進行處理（例如提交表單或者上傳檔案）。資料被包含在請求本文中。 |
| PUT | 向指定資源位置上傳其最新內容。 |
| DELETE | 請求伺服器刪除Request-URI所標識的資源。 |
| TRACE | 回顯伺服器收到的請求，主要用於測試或診斷。 |
| OPTIONS | 這個方法可使伺服器傳回該資源所支援的所有HTTP請求方法。用'*'來代替資源名稱，向Web伺服器傳送OPTIONS請求，可以測試伺服器功能是否正常運作。 |
| CONNECT | HTTP/1.1協定中預留給能夠將連接改為隧道方式的代理伺服器。通常用於SSL加密伺服器的連結（經由非加密的HTTP代理伺服器）。 |

超文本傳輸協定（英語：HyperText Transfer Protocol，縮寫：HTTP）是一種用於分佈式、協作式和超媒體訊息系統的```應用層```協定
- 設計HTTP最初的目的是為了提供一種發布和接收HTML頁面的方法。透過HTTP或者HTTPS協定請求的資源由[統一資源識別碼（Uniform Resource Identifiers，URI）](https://zh.wikipedia.org/wiki/%E7%BB%9F%E4%B8%80%E8%B5%84%E6%BA%90%E6%A0%87%E5%BF%97%E7%AC%A6)來標識。
## 統一資源識別碼
- URI可被視為定位符（URL），名稱（URN）或兩者兼備。統一資源名（URN）如同一個人的名稱，而統一資源定位符（URL）代表一個人的住址。換言之，URN定義某事物的身分，而URL提供尋找該事物的方法。
用於標識唯一書目的ISBN系統是一個典型的URN使用範例
