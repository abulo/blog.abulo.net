title: 自学 Golang 第一课(语言基础)
author: Abulo Hoo
tags: []
categories:
  - Golang
date: 2019-01-06 19:41:00
---
** Go标识符 **

标识符是用来干什么的?

标识符是用来命名变量,类型等内容,标识符由字母(A-Z 或者 a-z),数字(0-9),下划线组成,特别需要注意的是第一个必须是字母或者下划线,标识符不允许使用系统内置的关键字

** Go关键字 **

|break|default|func|interface|select|
|:---|:---|:---|:---|:---|
|case|defer|go|map|struct|
|chan|else|goto|package|switch|
|const|fallthrough|if|range|type|
|contiue|for|import|return|var|

**Go预定义标识符**

|append|copy|int8|nil|true|
|:---|:---|:---|:---|:---|
|bool|delete|int16|panic|uint|
|byte|error|int32|print|uint8|
|cap|false|int64|println|uint16|
|close|float32|iota|real|uint32|
|complex|float64|len|recover|uint64|
|complex64|imag|make|rune|uintptr|
|complex128|int|new|string||


**常量和变量**

常量使用 `const` 声明,变量使用 `var` 声明,也可以使用快捷键变量声明,Go可以根据变量的内容自动判断变量类型.


```code
const limit = 512	//常量,其类型兼容任何数字
const top uint16 = 1421	//常量,类型:uint16
start := -19	//变量,类型判断int
end := int64(9876543210)	//变量,类型int64
var i int	//变量,类型int,默认值 0
var debug = false //变量,类型bool
checkResults := true //变量,类型bool
j := 1.5 //变量,类型float64
s := "string" //变量,类型string
```

对于整型字面量 Go 推断为 int,对于浮点型字面量 Go 推断为 float64,对于复数型字面量 Go 推断为 complex128 

变量 i 未初始化,Go 会将 0 赋值给该变量,
如果该变量声明的是一个未初始化的字符串,Go会将空字符赋值给该变量





