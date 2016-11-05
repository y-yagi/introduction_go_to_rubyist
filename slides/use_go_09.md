
## 性能比較

* 名前とemailが含まれるユーザデータをJSONで返すAPIをRubyとGoそれぞれで作成
  * データ件数は100件
* Siegeで同時ユーザー数50、リクエスト数100で負荷を掛けてみた
* DBはPostgreSQL
