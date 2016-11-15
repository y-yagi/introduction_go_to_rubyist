
## 性能比較

* 名前とemailが含まれるユーザデータをJSONで返すAPIをRubyとGoそれぞれで作成
  ```
  "id":1,"name":"dummy_0","email":"dummy_0@example.com",
  "created_at":"2016-10-29T06:43:05.399952Z","updated_at":"2016-10-29T06:43:05.399952Z"}
  ```
  * データ件数は100件
* DBはPostgreSQL
* Siegeでユーザー数50 * リクエスト数200 = 合計10,000リクエスト実行
