# Python class on NTU
###### tags: `Python` `NTU`

:::info
Alt+P : Shell recall 上次指令
:::

---

### - IDLE -
> File -> New File
> Run -> Run Module

### - Coding -
* BIG-5 繁體中文
* UTF-8 Unicode
> 1. Python 3.x default
> 2. Python 2.x 需要設定
> `# -*- coding: utf-8 -*-`
> Or
> `# coding: utf-8`

![](https://i.imgur.com/7DcV9iO.png)

### - 資料型態 -
* 數值型別: `int`, `float`, `bool`, `complex`
> bool : True, False, None
> complex : 虛數
* 字串型別: `str`
* 容器型別: `tuple`, `list`, `set`, `dict`
> Container Type - 
> 1. tuple : 序對 (元組) ; "( )" ; 有順序 ; 不可更改內容
> 2. list : 串列 (清單) ; "\[ \]" ; 有順序 ; 可修改內容
> 3. set : 集合 ; "{ }" ; 無順序 ; 可修改內容
> 4. dict : 字典 ; "{ }" ; Key-Value ; 可修改內容

### - 函式 -
**built-in function**
1. type() : 回傳變數型態
2. input() : 回傳一定是string
3. eval() : 字串轉數字
4. int() : 字串轉數字
5. range() : range(\[start\],stop,\[step\])

:::danger
eval 危險語法，使用上要小心!!
:::
:::info
`range(\[start\],stop,\[step\])`
start: 起始值, default=0
stop: 停止條件
step: 迭代數字, default=1, 可以用負數
:::

---
:::info
Python裡面所有東西都是object
:::

:::info
宣告str的變數內容不可改變
:::

---
### - 賦值 -
```python=
x = 12 # ==> 把 12 賦值給 x
```

---
:::info
* "in" 適用於: 字串、集合、清單、序對
* "in" 用在Dictionary, 只比對Key值, 非Value值
* Python以縮排來區分程式碼區塊, 縮排沒有對齊, 執行會出現錯誤
* 空白鍵與Tab鍵不同
:::

---
### - 數字系統 -
* Integer
* Float
* 方法: `bin()`, `oct()`, `hex()`

### - 字串系統 -
* strip() : 去除左右兩側(頭尾)空白或是溢出字元('\n', '\t', ...etc)
* lstrip() : 去除左側空白
* rstrip() : 去除右側空白
* capitalize() : 第一個字元變大寫
* title() : 每個單字的第一個字元變大寫
* swapcase() : 大小寫互換
* upper()
* lower()
* ==sort()== ==> integer
* ==translate()== & ==maketrans()== : 字元轉換
* ==zfill(\<width\>)== : 字串補'0', 長度Width
* endswith()
* startswith()
* istitle()
* isupper()
* isdigit()
* isspace()

:::info
用法
1. str.upper(\<string\>)
2. \<string\>.upper()

PS: 字串方法不會改變字串內容
:::
```python=
# 練習
s3 = "Hello, world!"
print(s3.zfill(17))
print('0' * 8 + s3)
```

---
:::info
物件.方法() ==> object.method()
:::

---
