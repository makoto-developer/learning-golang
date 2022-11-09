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
var job string = "programmer"
```

## if

```go
if job == "programmer" {
	fmt.Println("your job is %s", job)
}
```

## 配列

```go
nameList = []string{"john", "alice", "jane"}
```

## for

```go
// i is number
for i, name := range nameList {
    fmt.Println("member is %s. No.%d", name, i)
}
```

## 関数

```go

```