
## 性能比較

* Rails以外に、[Sequel](http://sequel.jeremyevans.net/) + [Roda](http://roda.jeremyevans.net/)のパターンを追加
* APサーバはPuma
  * puma configはRailsアプリと同じ内容
* JSON への変換はSequelデフォルトの変換処理を使用(外部 gemは使用せず)
