## http
[HyperText Transfer Protocol](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol)

[超文本傳輸協議](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE)

超文本傳輸協定（英語：HyperText Transfer Protocol，縮寫：HTTP）是一種用於分佈式、協作式和超媒體訊息系統的```應用層```協定
- 設計HTTP最初的目的是為了提供一種發布和接收HTML頁面的方法。透過HTTP或者HTTPS協定請求的資源由[統一資源識別碼（Uniform Resource Identifiers，URI）](https://zh.wikipedia.org/wiki/%E7%BB%9F%E4%B8%80%E8%B5%84%E6%BA%90%E6%A0%87%E5%BF%97%E7%AC%A6)來標識。
## 統一資源識別碼
- URI可被視為定位符（URL），名稱（URN）或兩者兼備。統一資源名（URN）如同一個人的名稱，而統一資源定位符（URL）代表一個人的住址。換言之，URN定義某事物的身分，而URL提供尋找該事物的方法。
- 用於標識唯一書目的ISBN系統是一個典型的URN使用範例
                  hierarchical part
        ┌───────────────────┴─────────────────────┐
                    authority               path
        ┌───────────────┴───────────────┐┌───┴────┐
  abc://username:password@example.com:123/path/data?key=value&key2=value2#fragid1
  └┬┘   └───────┬───────┘ └────┬────┘ └┬┘           └─────────┬─────────┘ └──┬──┘
scheme  user information     host     port                  query         fragment

  urn:example:mammal:monotreme:echidna
  └┬┘ └──────────────┬───────────────┘
scheme              path
