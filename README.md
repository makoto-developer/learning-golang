# Go言語 文法

## 型

論理値型

|型|値| note |note|
|:----|:----|:-----|
|bool|true, false||

数値型

| 型      |値| note |
|:-------|:----|:-----|
| int8   |-128 ～ 127||
 | int16  |-32768 ～ 32767||
 | int32  |-2147483648 ～ 2147483647||
 | int64  |-9223372036854775808 ～ 9223372036854775807||
 | int    |32bit または 64bit (環境依存)||
 | unit8  |0 ～ 255||
 | unit16 |0 ～ 65535||
 | unit32 |0 ～ 4294967295||
 | unit64 |0 ～ 18446744073709551615||
 | unit   |32bit または 64bit|環境依存|

浮動小数点型

|型|値| note |note|
|:----|:----|:-----|
|float32|32ビット||
|float64|64ビット||

文字列型

|型|値| note |note|
|:----|:----|:-----|
|string|文字列||

## 変数宣言

```go
// basicな書き方
var job string = "programmer"

// ↑の省略形
job string = "doctor"

// 再代入禁止
job string := "student"

```

## if

```go
if job == "programmer" {
	fmt.Println("your job is %s", job)
}
```

## 比較

```go
a == b 
a != b 
a > b  
a >= b 
a < b  
a <= b 
a && b 
a || b
!a
```


## 配列

```go
// string array
nameList = []string{"john", "alice", "jane"}

// number array
scores = []int32{10, 32, 49, 44, 95}
```

## for

```go
go i:=0; i<10; i++ {
	// 処理を記述
}
```

```go
// i is number
for i, name := range nameList {
    fmt.Println("member is %s. No.%d", name, i)
}
```

## 構造体

```go
type Person struct {
     name: string,
	 age: uint8,
     address: string
}
```

## 関数

```go
func getPerson(name string) (Person) {
	person := Person{
		name: name,
		age: 10,
		address: string
    }
	
	return person
}
```

## ポインタ

変数はメモリ上に記録されている。
そのアドレスを取得するには`&変数`で取得できる。
ポインタ型変数を定義するには`*変数`で定義できる。

```go
name *string = &name

// 値を更新する
*name = "bob"
```

