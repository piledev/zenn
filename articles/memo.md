# 書きたいこと
## 2021.09.18
1. test でエラーを発生させる手段
```go
	err := dispatchError()
	// これって本当にキャスト?
	// -> type assertion というものらしい。
	// interface (型の決まっていないもの) を()内の型にキャストしたいときに使うものらしい
	// type assersion のキャストって、構成が同じだけでは失敗するっぽい
	// error の内容がそれじゃないと
	me, ok := err.(*mysql.MySQLError)
```
