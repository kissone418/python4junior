# 學習單元
```
[1]函數
[2]函式的參數 與 回傳的咚咚
[3]變數的有效範圍(Scope)
[4]各種函數技術
   匿名函數
   遞迴函數(長大一點後以後再學)
[5]Python 內建函數(Built-in Functions)
```
# [1]函數開發初體驗
```
def sum(i1, i2):
    result = 0
    for i in range(i1, i2):
        result += i
    return result

def main():
    print("Sum from 1 to 10 is", sum(1, 11)) 
    print("Sum from 20 to 37 is", sum(20, 38))
    print("Sum from 35 to 49 is", sum(35, 50))

main() # Call the main function
```
## 函式的定義:
```
函數代碼塊以 def 關鍵字開頭，後接函數識別字名稱和圓括號()。
任何傳入參數和引數必須放在圓括號中間。圓括號之間可以用於定義參數。
函數的第一行語句可以選擇性地使用文檔字串—用於存放函數說明。
函數內容以冒號起始，並且縮排。
return [運算式] 結束函數，選擇性地返回一個值給調用方。不帶運算式的return相當於返回 None。
函式包含標頭和主體。
標頭(header)起源於def關鍵字，後接函式名稱和參數，最後以冒號結尾。
```

```
【Python 練習實例47】練習撰寫swap(a,b)函式
                    寫一個函式將輸入的兩個變數值互換
```

```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
def swap(a,b):
    a,b = b,a
    return (a,b)
 
if __name__ == '__main__':
    x = 10
    y = 20
    print('x = %d,y = %d' % (x,y))
    x,y = swap(x,y)
    print('x = %d,y = %d' % (x,y))
```


# [2］函式的參數 與 回傳的咚咚

```
Python的函式是否有無回傳值，端視函式是否有無return敘述。

若函式沒有回傳值，預設是回傳一None特殊值。
因此，沒有回傳值的函式也稱為None函式。
None值可以指定給一變數，表示此變數沒有參考到任何的物件
```

## Python的函數可以回傳多個值(超棒der)
```
#!/usr/bin/python 
# -*- coding: UTF-8 -*- 

def sort(number1, number2):
    if number1 < number2:
        return number1, number2
    else:
        return number2, number1

num1, num2 = sort(31, 25)

print("num1 is", num1)
print("num2 is", num2)

### [作業]:def sort(number1, number2, number3):
```
# 更多函式與參數 ... ==>
```
Default arguments預設參數
Positional arguments位置參數
Keyword arguments關鍵字參數
```

# [3]變數的有效範圍 {就是你電動的  勢力範圍}
```
變數的有效範圍(Scope)：變數在程式可參考的範圍。

區域變數(local variable):宣告在函式內部的變數
全域變數(global variables):宣告在所有函式外部的變數
```
```
x = 111   # x是 ===> 問題1: [1]區域變數(local variable)   [2]全域變數(global variables)

def f1():
    x = 222    # 問題2: [x是 ===>  [1]區域變數(local variable)   [2]全域變數(global variables)
    print(x)   # 問題3: [答案是多少??

f1()
print(x)        # 問題4: [答案是多少??
```

```
x = 1

def increase():
    global x
    x =  x + 1
    print(x) 

increase()
print(x)
increase()
increase()
print(x)
```
# [4] 各種函數技術

## 匿名函數==>lambda 運算式
```
匿名函數==沒有函數名稱、臨時使用的小函數
使用lambda 運算式來宣告匿名函數
lambda 運算式只能包含一個運算式， 不允許複雜的語句，但運算式中可呼叫其他函數
```

### 把lambda運算式當做函數
```
f1 = lambda x, y, z: x+2*y+3*z
print(f1(2,3,1))
```

### 在lambda 運算式中呼叫其他函式(重要技術)
```
# 定義要處理的函數
def myfunc(m):
    return m*m

# 原始資料
my_list = [1, 3, 5, 7, 9]

#使用python的map()套用

print(list(map(lambda x:myfunc(x), my_list)))
```

# [5]Python 內建函數==>Built-in Functions:

```
https://docs.python.org/3.8/library/functions.html
https://www.programiz.com/python-programming/methods/built-in
```

### hex(x):Convert an integer number to a lowercase hexadecimal string prefixed with “0x”
```

hex(255)

hex(-42)

```
### oct(x):Convert an integer number to an octal string prefixed with “0o”"
```
oct(8)

oct(-56)

```
### bin(x):Convert an integer number to a binary string prefixed with “0b”
```
bin(3)

bin(-10)
```
