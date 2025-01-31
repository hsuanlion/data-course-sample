# Q1: Mimi Beauty 遇到的問題是什麼？
- 推動Mini Beauty平台營收成長的重要因素來自網路流量，而流量則主要是透過數位廣告CPC獲取的，且佔訂單超過30%。整體流量雖然增加，但轉換率和客單價卻持平。因此如何將數位廣告導入到平台上的流量有效變現，是Mini Beauty目前需要解決的問題。


# Q2: 推薦系統能解決什麼問題？
1. 商品頁面推薦清單，可以解決轉換率問題。透過推薦清單，幫助客戶在上千商品SKU中找到可能會喜歡的商品，進而降低選擇障礙，提高轉換機會。
2. 結帳頁面的推薦清單，可以解決客單價問題。透過推薦推薦清單，幫助客戶在結帳頁面可以再看到其他可能喜歡商品，進而提高客單價。



# 「Rule-based」的推薦系統實作方法說明

測試了以下Rule-based推薦規則
1. 每個人隨機推薦10樣商品
- 推薦分數score: 0.006779661016949152
2. 每人都推薦2018-09月以前，平均分數前10名商品
- 推薦分數score: 0 
3. 每人都推薦2018-09月以前，評論次數前10名商品
- 推薦分數score: 0.08305084745762711
4. 每人都推薦有史以來，銷售排名前10名商品
- 推薦分數score: 0.005084745762711864

# 「Rule-based」的推薦系統結果
其中以每人都推薦2018-09月以前，評論次數前10名商品的規則得到的score效果最好(0.0831)，相較於隨機推薦10件商品的分數(0.0068)，lift為11倍(0.0831/0.0068 - 1 = 11.22)。表示使用期間有很多人買、討論度高的熱銷商品做推薦時，會有不錯的效果。







