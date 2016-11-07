
## goroutine / channel

* 軽量スレッド?
  * OSスレッドと異なり、goroutineのデフォルトスタックのサイズは大分小さい(2KB。OSスレッドは2MBとか)
  * goroutineのスタックは必要に応じて拡大したり縮小したりするようになっている(らしい)
