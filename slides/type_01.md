
## 型(整数)

* 整数
  * 符号付き整数: int8, int16, int32, int64, int
  * 符号無し整数: uint8, uint16, uint32, uint64, uint
  * rune(int32ｎシノニム。値がUnicodeのコードポイントである場合に使用する事がおおい)
  * byte(uint8のシノニム)
  * uintptr(ポインタ用)
  * int, uintは同じサイズであり、32bit or 64bit
  * どちらになるかはハードウェアやコンパイラに依存する
