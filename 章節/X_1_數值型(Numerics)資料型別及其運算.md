
# 數值型資料型別(Numerics Data Type)
```
[1]Python支援的數值型資料型別(Numerics Data Type)
[2]基本的運算
算術運算子Arithmetic operators
比較（關係）運算子Comparison operators
賦值運算子Assignment operators
邏輯運算符Logical operators
位元運算子Bitwise operators
成員運算子Identity operators
身份運算子Membership operators

運算子優先順序

[3]內建的各種數學函數(Built-in functions)
[4]練習題
```
# [1]Python支援的數值形資料型別(Numerics Data Type)
```
# Python 支持三種不同的數值型別(Data Type)：

[1]Int 整數，是可以是正或負整數，不帶小數點。
   Python3  int是沒有限制大小的，可以當作 Long 類型使用，所以 Python3 沒有 Python2 的 Long 類型。

[2]浮點數(float) :由整數部分與小數部分組成，浮點型也可以使用科學計數法表示（2.5e2 = 2.5 x 10 0 = 250）

[3]複數( (complex)) - 複數由實數部分和虛數部分構成，可以用a + bj,或者complex(a,b)表示， 複數的實部a和虛部b都是浮點型。

https://www.w3schools.com/python/python_exercises.asp
```
```
x = 1
y = 2.8
z = 1j

print(type(x))
print(type(y))
print(type(z))
```
# [2]數值型別(Numerics Data Type)的各種運算

### 動手完成底下的練習
```
底下以範例快速示範
同學請勤作練習,完成你自己的python學習之路
https://www.w3schools.com/python/python_operators.asp
```
### 算術運算
```
a = 17 / 3

b = 17 // 3

c = 17 % 3

a,b,c
```
```
a = 7//2
b = 7.0//2
c = 7//2.0

a,b,c
```

```
5 ** 2
-3%2
```

### _
```
tax = 12.5 / 100
price = 100.50
price * tax

price + _

round(_, 2)

round(_)
```
### Logical Operators 邏輯運算
```
x = 5

print(x > 3 and x < 10)

x = 5

print(x > 3 or x < 4)

x = 5

print(not(x > 3 and x < 10))
```
### Bitwise Operators 位元運算[略]

## 進位制:
```
number1 = 0b1000111
number1

number2 = 0xA0F
number2

number3 = 0o37 
number3
```
# [3]各種數學函數
```
https://www.w3schools.com/python/python_ref_functions.asp

### 作業:完成十種函數的自我測試報告
```
### 數字系統的轉換
```
x = bin(36)
x
```
```
y = oct(36)
y
```
```
z = hex(255)
z
```
### int()函數的測試
```
https://www.w3schools.com/python/ref_func_int.asp
```
```
x=int('10',2)
x
```
```
x=int('10',16)
x
```
```
x=int('10',8)
x
```
### round()函數的測試
```
#Round a number to only two decimals:

x = round(5.76543, 2)
print(x)
```
```
# Round to the nearest integer:

x = round(5.76543)
print(x)
```
### Python 類型轉換
```
有時候，我們需要對資料內置的類型進行轉換，

資料類型的轉換只需要將資料類型作為函數名即可。

int(x) ==>將x轉換為一個整數。
float(x) ==> 將x轉換到一個浮點數。
complex(x) ==>將x轉換到一個複數，實數部分為 x，虛數部分為 0。
```
```
complex(x, y) ===>將 x 和 y 轉換到一個複數，實數部分為 x，虛數部分為 y。x 和 y 是數字運算式。
```
```
a = 1.0004
int(a)
```
```
b = 0.9999
int(a)
```
# picoCTF 2017 : compute-rsa-50
```
RSA encryption/decryption is based on a formula that anyone can find and use, 
as long as they know the values to plug in. 
Given the encrypted number 150815, d = 1941, and N = 435979, what is the decrypted number?

HINTS
decrypted = (encrypted) ^ d mod N
```
# 思考提
```
輸入一個5位數，撰寫程式判斷它是不是回文數。
即12321是回文數，個位與萬位相同，十位與千位相同。
```
```
輸入一個數，判斷該數是否是迴文數？
```
