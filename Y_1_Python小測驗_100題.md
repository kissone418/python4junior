# Python小測驗_100題
# 1.Python入門
```
1.要在螢幕輸出Hello, Python!  底下程式需使用哪個函數:

#!/usr/bin/python3
________("Hello, Python!")

(A) print   (B) printf   (C) printline   (D) printn
```
```
2.要在程式碼中新增一行註解，底下程式需使用哪個符號:

#!/usr/bin/python3
__這是一行註解
print("Hello, Python!")

(A)	/   (B) -   (C) #   (D) <!-->
```
```
3.要新建一個變數名稱為school，並將變數值設定為ksu，底下程式需填入:

#!/usr/bin/python3
(1)______ = “(2)______”

(A) (1)ksu，(2)school    (B) (1) school，(2) ksu  
(C) (1)”ksu”，(2)school   (D) (1)ksu，(2)”school”  
```
```
4.要檢查變數資料型別 底下程式需使用哪個函數:

#!/usr/bin/python3
y = 65535
print(______(y))

(A) str   (B) sum   (C) int   (D)type

```
```
5.試問以下程式執行後輸出什麼:

#!/usr/bin/python3
y = 65535
print(type(y))

(A) <class 'int'>  (B) <class 'str'>  (C) <class 'float'>  (D) <class 'tuple'>
```
```
6.要在程式碼中進行資料型態轉換 底下程式需使用哪個函數將x轉換成float:

#!/usr/bin/python3
x = 65535
______(x)

(A) long   (B) str   (C) float   (D)int
```
```
7.要計算一個字串長度 底下程式需使用哪個函數:

#!/usr/bin/python3
string1 = "Hello, Python!"
print(___________(string1))

(A) find   (B) len   (C) count   (D)replace
```
```
8.試問以下程式執行後輸出什麼結果:

#!/usr/bin/python3
print(100 < 200)

(A) False   (B) True   (C) 100   (D) 200
```
# 2.資料型態及其運算 DataType
```
9.要定義一個整數變數a  底下程式碼需填入什麼:
#!/usr/bin/python3
a = ___________

(A) 1
(B) 1.0
(C) 100 / 10
(D) 1.0 * 1.0
```
```
10.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = bool(100)
print(a)

(A) 0
(B) 100
(C) False
(D) True
```
```
11.要在螢幕輸出變數x的資料型態  底下程式需使用哪個函數:
#!/usr/bin/python3
a = 100
print(_______(a))

(A) any   (B) type   (C) complex   (D) bin
```
```
12.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = “Python!”
print(type(a))

(A) str   (B) int   (C) float   (D) tuple
```
```
13.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = ("Python", True, 1234)
print(type(a))

(A) str   (B) int   (C) float   (D) tuple
```
```
14.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = ["Python", "True", "1234"]
print(type(a))

(A) set   (B) dict   (C) list   (D) tuple
```
```
15.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = {"name" : "Eric", "age" : 90}
print(type(a))

(A) set   (B) dict   (C) list   (D) tuple
```
## 字串1
```
16.試問若要定義一字串變數應填入什麼:

#!/usr/bin/python3
a = ________
print(a)

(A) "Hello Python"
(B) <Hello Python>
(C) [Hello Python]
(D) {"Hello Python"}
```
```
17.試問以下程式執行後輸出什麼結果:

#!/usr/bin/python3
a = "Hello, World!"
print(a[1])

(A) H   (B) e   (C) l   (D) 1
```
```
18.要在螢幕輸出llo  底下程式需填入什麼:

#!/usr/bin/python3
a = "Hello, World!"
print(a[__________])

(A) 4:6   (B) 3:5   (C) 2:5   (D) llo
```
```
19.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = "        HelloPython "
print(a.strip())

(A) HelloPython
(B)        HelloPython
(C) HelloPython         
(D) H e l l o P y t h o n
```
```
20.試問若要判斷Kun是否存在於txt字串中以下程式應填入什麼:
#!/usr/bin/python3
txt = " Kun Shan University was officially founded on April 29, 1965"
x = "Kun" __________ txt
print(x) 

(A) is
(B) on
(C) ==
(D) in
```
```
21.試問若要輸出a、b兩字串合併後的結果以下程式應填入什麼:
#!/usr/bin/python3
a = “Kun Shan”
b = “University”
print(__________)

(A) a & b
(B) a + b
(C) ab
(D) a,b
```
```
22.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = “Kun Shan”
b = 100
print(a + b)

(A) Kun Shan100
(B) a + b
(C) 100 Kun Shan
(D) TypeError
```
## 字串2
```
23.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = 'Kun Shan {}'
b = 'University'
print(a.format(b))

(A) Kun Shan {}
(B) Kun Shan University
(C) University Kun Shan
(D) University
```
```
24.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
a = '{1} Kun Shan {0}'
b = 'University'
print(a.format(b,‘Hello’))

(A) Hello Kun Shan University
(B) University Kun Shan Hello
(C) {1} Kun Shan {0}
(D) b,‘Hello’
```
```
25.試問若以下程式執行後要輸出一對雙引號需填入什麼:
#!/usr/bin/python3
a = “_____________”
print(a)

(A) “”
(B) <””>
(C) \"\"
(D) [“”]
```
```
26.要在螢幕輸出字串的長度  底下程式需使用哪個函數:
#!/usr/bin/python3
a = “Kun Shan”
print(_______)

(A) len(a)
(B) length(a)
(C) abs(a)
(D) int(a)
```
```
27.試問要英文字母轉為大寫以下程式需填入什麼:
#!/usr/bin/python3
a = “Python”
print(__________)

(A) a. isupper()
(B) a. islower()
(C) a.upper()
(D) a.lower()
```
```
28.試問以下程式執行後輸出什麼結果:
#!/usr/bin/python3
print(“%s Python! %d” % (“Hello”,123))

(A) “%s Python! %d” % (“Hello”,123)
(B) 123 Python! Hello
(C) %s Python! %d
(D) Hello Python! 123
```
```
29.若要將字串a中的o替換成x以下程式需填入什麼:
a = “Hello Python!”
a = a._________
print(a)

(A) replace(“o”,”x”)
(B) replace(“x”,”o”)
(C) “Hellx Pythxn!”
(D) format(“o”,”x”)
```
# 3.選擇結構1
```
30.
if None:
    print("Hello")
以上程式碼輸出的結果是？

(A) 沒有任何輸出
(B) 語法錯誤
(C) Hello
(D) False
```
```
31.
if 1:
    print("Hello")
以上程式碼輸出的結果是？

(A) 沒有任何輸出
(B) 語法錯誤
(C) Hello
(D) False
```
```
32.
if 100:
    print("Hello")
以上程式碼輸出的結果是？

(A) 沒有任何輸出
(B) 語法錯誤
(C) Hello
(D) False
```
```
33.
if 0:
    print("Hello")
以上程式碼輸出的結果是？

(A) 沒有任何輸出
(B) 語法錯誤
(C) Hello
(D) False
```
```
34.
if 100 == “100”:
    print("Hello")
以上程式碼輸出的結果是？

(A) 沒有任何輸出
(B) 語法錯誤
(C) Hello
(D) False
```
```
35.
if 100 == 100:
    print("Hello")
以上程式碼輸出的結果是？

(A) 沒有任何輸出
(B) 語法錯誤
(C) Hello
(D) False
```
```
36.
if 100 >= 1:
    print("Hello")
以上程式碼輸出的結果是？

(A) 沒有任何輸出
(B) 語法錯誤
(C) Hello
(D) False
```
## 選擇結構2
```
37.
a = 100
b = 50
if ________:
  print("Hello Python!")
else:
  print("Hello World!")
若要讓程式印出Hello World!需在___中填入什麼？

(A) a == b、a < b、a <= b
(B) a != b
(C) a
(D) b
```
```
38.
a = 50
b = 1000
print("A") if a > b else print("B")
以上程式碼輸出的結果是？

(A) b
(B) a
(C) B
(D) A
```
```
39.
a = 50
b = 51
print("A") if a > b else print("B") if a != b else print("!=")
以上程式碼輸出的結果是？

(A) A
(B) !=
(C) B
(D) 語法錯誤
```
```
40.
a = 77
b = 10
c = 0
if a > b ___ c > a:
  print("True")
若要讓程式印出Hello World!需在___中填入什麼？

(A) not in
(B) not
(C) or
(D) and
```
```
41.
a = 0
b = a + 10

if b > a:
  ______
若要讓程式成功編譯執行應填入什麼？

(A) pass
(B) return 0
(C) return True
(D) break
```
```
42.
x = 10
if x >= 10:
  if x > 20:
    print("1")
  else:
    print("2")
以上程式碼輸出的結果是？

(A) 10
(B) 1
(C) 2
(D) 0
```
```
43.
a = 33
b = 32
x = 10
if b > a:
  print("b > a")
elif a == b:
  if x >= 10:
    if x > 20:
      print("1")
    else:
      print("2")
      
(A) b > a
(B) 2
(C) 1
(D) 沒有任何結果
```
## List
```
44.
cat = ______
創建一個cat的串列需填入什麼？

(A) [“Python”,”C”,”JAVA”,” Assembly”]
(B) {'a': 1, 'b': 2, 'b': '3'}
(C) new cat;
(D) list()
```
```
45.
thisislist = [1,2,3,4,5]
print(__________)
輸出list中的第3個元素需填入什麼？

(A) thisislist(3)
(B) thisislist(2)
(C) thisislist[3]
(D) thisislist[2]
```
```
46.
thisislist = [1,2,3,4,5]
print(thisislist[-4])
以上程式碼輸出的結果是？

(A) 1
(B) 2
(C) 3
(D) 4
```
```
47.
thisislist = [1,2,3,4,5]
print(thisislist[_________])
若要以上程式碼輸出的結果是2,3,4需要填入什麼？

(A) 1:4
(B) 1:3
(C) 1-4
(D) 1-3
```
```
48.
thisislist = [1,2,3,4,5]
print(thisislist[-5:-3:2])
以上程式碼輸出的結果是？

(A) 1
(B) 2
(C) 3
(D) 4
```
```
49.
thisislist = [1,2,3,4,5]
________ = 100
print(thisislist)
若需變更第四個元素為100需要填入什麼？

(A) thisislist(4)
(B) thisislist(3)
(C) thisislist[4]
(D) thisislist[3]
```
```
50.
thisislist = [1,2,3,4,5]
__________
若需在list後方加入一元素6要填入什麼？

(A) thisislist.append(6)
(B) thisislist.add(6)
(C) thisislist.insert(6)
(D) thisislist[5] = 6
```
## Dictionary 資料型態
```
51.
thisisdict = ________
建立一個字典變數需填入什麼？

(A) [“Python”,”C”,”JAVA”,” Assembly”]
(B) {'a': 1, 'b': 2, 'c': 3}
(C) dict()
(D) 123456
```
```
52.
thisisdict = {'a': 1, 'b': 2, 'c': 3}
x = ___________
print(x)
要取出b的值需填入什麼？

(A) thisisdict[b]
(B) thisisdict["2"]
(C) thisisdict["b"]
(D) thisisdict[b]
```
```
53.
thisisdict = {'a': 1, 'b': 2, 'c': 3}
______ = 100
print(thisisdict)
若需改變b的值需填入什麼？

(A) thisisdict[b]
(B) thisisdict["2"]
(C) thisisdict["b"]
(D) thisisdict[b]
```
```
54.
thisisdict = {'a': 1, 'b': 2, 'c': 3}
if “3” in thisisdict:
   print(“Yes”)
以上程式碼輸出的結果是？

(A) Yes
(B) No
(C) True
(D) 沒有輸出結果
```
```
55.
thisisdict = {'a': 1, 'b': 2, 'c': 3}
if “a” in thisisdict:
   print(“Yes”)
以上程式碼輸出的結果是？

(A) Yes
(B) No
(C) True
(D) 沒有輸出結果
```

```
56.
thisisdict1 = dict(a="1", b="2", c=3)
print(thisisdict1)
以上程式碼輸出的結果是？

(A) 語法錯誤
(B) {'a': '1', 'b': '2', 'c': 3}
(C) {}
(D) {'1': 'a', '2': 'b', '3': c}
```
```
57.
thisisdict1 = dict(a="1", b="2", c=3)
thisisdict1.pop(“b”)
print(thisisdict1)
以上程式碼輸出的結果是？

(A) {'a': '1', 'c': 3}
(B) {'a': '1', 'b': '2', 'c': 3}
(C) ['a': '1', 'c': 3]
(D) ['a': '1', 'b': '2', 'c': 3]
```
# Loop迴圈
## while迴圈1
```
58.
i = 20
while i < 60:
  print(i)
  i -= -1
以上程式碼最後輸出的結果是？

(A) 59
(B) 60
(C) 20
(D) 0
```
```
59.
i = 20
while i < 60:
  i -= -1
print(i)
以上程式碼輸出的結果是？

(A) 59
(B) 60
(C) 20
(D) 0
```
```
60.
i = 20
while i == 20:
  print(“ok”)
以上程式碼輸出的結果是？

(A) 無窮迴圈，瘋狂輸出ok
(B) 輸出一次ok
(C) 程式不會輸出任何訊息
(D) 語法錯誤
```
```
61.
i = 20
while i == 20:
  print(“ok”)
  _________
執行以上程式碼只會輸出一次OK需填入什麼？

(A) end while
(B) return 0
(C) break
(D) return True
```
```
62.
i = 100
a = 0
while i >= 1 :
  a += i
  i += -1
print(a)
以上程式碼輸出的結果是？

(A) 5050，1加到100的總和
(B) 100
(C) 0
(D) -1
```
```
63.
i = 10
while i < 15:
  i += 1
  if i >= 13:
    continue
  print(i)
以上程式碼輸出的結果是？

(A) 15
(B) 13、14
(C) 10、11
(D) 11、12
```
```
64.
i = 1
_____ i < 3:
  print(i)
  i += 1
執行以上程式碼輸出的結果是1和2需填入什麼？

(A) True
(B) while
(C) for
(D) if
```
## for迴圈1
```
65.
________ x ______ [0, 1, 2]_____
  print(x)
以上程式碼使用for迴圈空格需依序填入什麼？

(A) for range :
(B) for list :
(C) for in {}
(D) for in :
```
```
66.
for x in [0, 1, 2]:
  print(x)
以上程式碼輸出的結果是？

(A) 0
(B) 0、1
(C) 0、1、2
(D) x
```
```
67.
for x in "Python for loop.":
  if _______:
    break
print(x)

(A) x == “Python”
(B) x == “ ”
(C) “ ” not in x
(D) x != “ ”
```
```
68.
for x in [0, 1, 2,3]:
  if x == 2:
    ________
  print(x)
以上程式碼輸出的結果是0、1、3需填入下列何者？

(A) continue
(B) break
(C) pause
(D) exit
```
```
69.
for x in range(6):
  print(x)
以上程式碼輸出的結果是？

(A) 輸出0~6
(B) 輸出0~5
(C) 輸出6
(D) 輸出隨機的6個數字
```
```
70.
for x in range(20, 15, _____):
  print(x)
若要讓以上程式碼輸出的結果都差距2需填入什麼？

(A) -2
(B) 2
(C) ++2
(D) 2++
```
```
71.
for x in [3,4,5]:
  ______
print(“ok”)
若要讓程式成功編譯執行應填入什麼？

(A) continue、pass、break
(B) return 0
(C) end
(D) 無法做到
```
# 函數Function
## 自訂函數1
```

72.
_______________:
  print("Hello print_function")
定義一個print_funtion需填入什麼？

(A) new print_funtion
(B) print_funtion()
(C) def print_funtion()
(D) DWORD print_funtion()
```
```
73.
def print_funtion():
  print("Hello print_function")

____________
若要呼叫print_funtion需填入什麼？

(A) call print_funtion;
(B) call print_funtion
(C) print_funtion()
(D) call print_funtion
```
```
74.
def add(a,b):
  return a+b

print(_______)
若要計算50+100以上程式碼需填入什麼？

(A) add(50,100)
(B) add(50+100)
(C) add(150)
(D) add()
```
```
75.
def print_name(yourname):
  print(yourname)

print_name ("Steve Jobs")
以上程式碼輸出的結果是？

(A) 語法錯誤
(B) print(yourname)
(C) yourname
(D) Steve Jobs
```
```
76.
def hello(greeting='Hello', name='world'): 
    print('{}, {}!'.format(greeting, name)) 

hello_3()
以上程式碼輸出的結果是？

(A) 沒有輸出
(B) Hello, world!
(C) greeting, name!
(D) '{}, {}!'.format(greeting, name)
```
```
77.
def hello(greeting='Hello', name='world'): 
    print('{}, {}!'.format(greeting, name)) 

hello_3('great', 'universe')
以上程式碼輸出的結果是？

(A) 沒有輸出
(B) Hello, world!
(C) great, universe!
(D) '{}, {}!'.format(greeting, name)
```
```
78.
def hello(greeting='Hello', name='world'): 
    print('{}, {}!'.format(name, greeting)) 

hello_3(name = 'great')
以上程式碼輸出的結果是？

(A) 沒有輸出
(B) Hello, world!
(C) '{}, {}!'.format(greeting, name)
(D) Hello, great!
```
## 匿名函數Lambda
```
79.
x = ___________
建立一個擁有參數與返回值y的Lambda函數需填入什麼？

(A) lambda y : y
(B) lambda y 
(C) lambda y : x
(D) lambda x : y
```
```
80.
x = lambda y : ______
建立一個擁有參數y與返回值自加100的Lambda函數需填入什麼？

(A) y+100
(B) x+100
(C) 100
(D) 0
```
```
81.
x = lambda y : y + 100
print(x(10))
以上程式碼輸出的結果是？

(A) 10
(B) 100
(C) 110
(D) 200
```
```
82.
x = lambda ___________
print(x(3, 3))
定義兩數相乘並有返回值的Lambda函數需填入什麼？

(A) a * b : a, b
(B) a, b : a * b
(C) a * b
(D) a, b
```
```
83.
def func(x):
  return lambda a : (2)________

a = func((1)_____)
print(a(8))
定義一個a函數使輸入的值能以7倍的值輸出需填入什麼？

(A) (1) 7  (2) a*x      (B) (1) a*x  (2) 7
(C) (1) 7  (2) a*a      (D) a*a    (2) 7
```
```
84.
def func(n):
  return lambda a : a * n

a = func(5)
print(a(10))
以上程式碼輸出的結果是？

(A) 100
(B) 50
(C) 150
(D) 25
```
```
85.
hard_func = lambda y, func: y + func(y)
hard_func (5, lambda y: y * y)
以上程式碼輸出的結果是？

(A) 5
(B) 25
(C) 30
(D) 100
```
### Python有許多內建函數(Built in Functions),底下考你對內建函數()的知識
### 參考來源:https://www.w3schools.com/python/python_ref_functions.asp
### 內建函數的小測驗:
```
86.
底下輸出結果為何?
abs(3+4J)

(A) 5.0   (B) 3.0   (C) 4.0   (D) 34.0
```
```
87.
底下輸出結果為何?

x = bin(37)
print(x)

(A) 0b100110    (B) 0b100101    (C) 0b110100   (D) 0b101100
```
```
88.
底下輸出結果為何?

x = chr(97)
print(x)
 
(A) a
(B) A
(C) B
(D) C
```
```
89.
底下輸出結果為何?

x = int(‘0xA’,16)
print(x)

(A) A
(B) 0xA
(C) 16
(D) 10
```
```
90.
底下輸出結果為何?

x = ”ksu university”
print(len(x))

(A) 12
(B) 13
(C) 14
(D) 15
```
```
91.
底下輸出結果為何?
x = [7,8,9,10]

print(max(x))

(A) 10
(B) 9
(C) 8
(D) 7
```
```
92.
底下輸出結果為何?
x = ord(“a”)
print(x)

(A) 123
(B) 321
(C) 0
(D) 97
```
```
93.
底下輸出結果為何?
a = 'print(100)'
eval(a) 

(A) 100   (B) 100.0   (C) print(100)   (D) TypeError
```
```
94.
底下輸出結果為何?

a = float(3)
print(a)

(A) 3    (B) 3.0    (C) a   (D) TypeError
```
```
95.
底下輸出結果為何?

a = hex(256)
print(a)
 
(A) 100
(B) 0x101
(C) 256
(D) 0x100
```
```
96.
底下輸出結果為何?

a = pow(2,3)
print(a)

(A) 8
(B) 6
(C) 4
(D) 2
```
```
97.
底下輸出結果為何?

a = pow(2,3,5)
print(a)

(A) 5
(B) 4
(C) 3
(D) 2
```
```
98.
底下輸出結果為何?
a = round(3.1415926,2)
print(a)

(A) 3.1415926
(B) 314
(C) 3.14
(D) 3.1
```
```
99.
底下輸出結果為何?
a = [5,6,8,3,2,1,7,4,9]
a = sorted(a)
print(a)

(A) [1, 2, 3, 4, 5, 6, 7, 8, 9] 
(B) [9, 8, 7, 6, 5, 4, 3, 2, 1]
(C) [5, 6, 8, 3, 2, 1, 7, 4, 9]
(D) [9, 4, 7, 1, 2, 3, 8, 6, 5]
```
```
100.
底下輸出結果為何?
a = divmod(5, 2)
print(a)

(A) (2, 1) 
(B) (2, 2) 
(C) (3, 1) 
(D) (3, 2)
```
