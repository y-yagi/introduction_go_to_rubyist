
## goroutine / channel

* Goのランタイムが一定数スレッドを起動し、空いてるスレッドに順番にgoroutineを載せて処理を進めていく
  * Go本体によりスケジューリングされる
* channelに対する操作はGo本体により排他制御が行われる　
  * 複数のgoroutineが同時にデータを読み込んだり書き込んだりはしない
* とはいえ、排他制御がまったく不要、という訳では無く、必要に応じてMutex を使う必要がある
