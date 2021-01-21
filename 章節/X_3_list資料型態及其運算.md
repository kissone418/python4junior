# 列表|串列(list)資料型態及其運算

```
[1]列表|串列(list)資料型態
[2]List的各種運算
  建立list
  使用索引(index)存取list元素

[3]list內建函數
[4]list的超強技法:
   序列拆解
   List comprehension 列表推導式
```
# [1]列表|串列(list)資料型態
```
list是最常用的Python資料類型，它可以作為一個方括號內的逗號分隔值出現。
list1 = [1, 2, 3, 4, 5 ]
list2 = ["a", "b", "c", "d"]

list的資料項目不需要具有相同的類型
list3 = ['linux', 'python', 1997, 2020]
```
```
序列是Python中最基本的資料結構。
序列中的每個元素都分配一個數字｜位置(索引index)，第一個索引是0，第二個索引是1，依此類推。

Python有6個序列的內置類型，但最常見的是列表(list)和元組(tuple)。
序列運算:序列都可以進行的操作包括索引，切片，加，乘，檢查成員。
內建函數|方法(Built-in Functions):Python已經內置確定序列的長度以及確定最大和最小的元素的方法。
```
```
Python Arrays??

Python does not have built-in support for Arrays, but Python Lists can be used instead.

For details please see below
https://www.w3schools.com/python/python_arrays.asp
```
# [2]List的各種運算
## 建立list
```
list1 = list() 
list1 = [] 

list2 = list([2, 3, 4])
list2 = [2, 3, 4] 

list3 = list(["red", "green", "blue"]) 
list4 = list(range(3, 6))
list5 = list("abcd") 
```
```
list1 = list() 
list1

list3 = list(["red", "green", "blue"])
list3

list4 = list(range(3, 6))
list4
```

## 使用索引(index)存取list元素
```
# List indexing

my_list = ['p', 'r', 'o', 'b', 'e']

# Output: p
print(my_list[0])

# Output: o
print(my_list[2])

# Output: e
print(my_list[4])
```

```
# 巢狀索引(Nested List)的使用

n_list = ["Happy", [2, 0, 1, 5]]

# Nested indexing
print(n_list[0][1])

print(n_list[1][3])
```
```
# Error! Only integer can be used for indexing
print(my_list[4.0])
```
```
# Negative indexing(負索引)的使用
my_list = ['H','a','p','p','y']

print(my_list[-1])

print(my_list[-5])
```

## List的各種運算(1)加法|乘法運算

```
下列範例會產生何種結果

list1 = [21, 23, 25]
list2 = [11, 92]

list3 = list1 + list2
list3
list4 = 3 * list1
list4
```

##  List的各種運算()切片運算(Slice)
```
list5 = list3[2:4]
list5
```

# [3]list內建函數:
```
加一元素到串列的尾端:append()
回傳元素x 出現於串列的次數:count()
附加在l中所有元素於串列:extend()
回傳在串列中第一次出現元素x的索引:index()
將串列中的元素加以反轉:reverse()
由小至大排序串列中的元素:sort()
```
###
```
下列範例會產生何種結果

list1 = [21, 33, 14, 12, 32,98]

len(list1)
max(list1)
min(list1)
sum(list1)


list1 = [21, 33, 14, 12, 32,98]
len(list1)
```

# [4]list的超強技法
## 序列拆解
"""

a=[12,212,321,325]
x,y,z,k = a
z

## List comprehension 列表推導式: list的超強大功能
```
A list comprehension consists of brackets containing an expression followed by a for clause, 
then zero or more for or if clauses. 
The result will be a new list resulting from evaluating the expression 
in the context of the for and if clauses which follow it. 

https://en.wikipedia.org/wiki/List_comprehension
```
```
list1 = [x for x in range(0,5)] 
list1

list2 = [0.5 * x for x in list1] 
list2

list3 = [x for x in list2 if x <= 1.5]
list3
```
### List comprehension列表推導式的應用

```
阿基米德與圓王比賽下棋， 國王說要是自己輸了的 話，阿基米德想要什麼他都可以拿得出來。 阿基米德說那就要點米吧！ 
棋盤一共 64 個小格子，在第一個格子放 l粒米，第二個格子放 2 粒米，第三個格子放 4 粒米，第四個格子放 8粒米，餘依此頡推，
後面每個格子的米都是前一個格子的 2 倍，一直把 64 個格子都放滿。

到底需要多少粒米呢
```
```
sum([2**i for i in range(5)])

sum([2**i for i in range(64)])
```
