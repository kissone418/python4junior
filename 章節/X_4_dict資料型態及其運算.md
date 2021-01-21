# dict資料型態及其運算
```
[1]dict資料型態
[2]dict資料型態及其運算
   建立dict的方法
[3]dict內建函數
   https://www.w3schools.com/python/python_ref_dictionary.asp
```

# [1]字典(Dictionary)
```
字典是一種可變容器模型，且可存儲任意類型物件。

字典的每個鍵值(key=>value)對用冒號(:)分割
每對pair之間用逗號(,)分割
整個字典包括在花括弧({})中


存取時:dict['Key']會得到value!
```
```
#!/usr/bin/python
 
dict = {'Name': 'Zara', 'Age': 7, 'Class': 'First'}
 
print("dict['Name']: ", dict['Name'])
print("dict['Age']: ", dict['Age'])


```
```
#### Queston 1:寫出上述dict的key有那些?

#### Queston 2:寫出上述dict的value有那些?

#### Queston 3:有幾組key-value pairs?
```
###  建立dict的方法
```
dict_1 = dict({"a":1234,"b":2345,"c":3456})
dict_1

dict_2 = dict(a=1234,b=2345,c=3456)
dict_2

dict_3 = {"a":1234,"b":2345,"c":3456}
dict_3
```
### 錯誤的寫法
```
dict_wrong = dict{"a":1234,"b":2345,"c":3456}
dict_wrong
```
### 存取字典的資料 How to access elements from a dictionary?
```
字典的key必須是唯一的
要取出value  使用中括號
```
```
dict_1["a"]
#dict_2["b"]
#dict_3["c"]
```
# [2]dict的運算

###  新增、修改、刪除與清除dict資料
```
#新增
dict_1["d"]=4567
dict_1

# 新增字典的key和value值::使用.setdefault()
data={"A":"123","B":"456"}
data.setdefault('C','789')
print(data)

#新增字典的key和value值使用.updata()
data={"A":"123","B":"456"}
dic2={"C":"987"}
data.update(dic2)
print(data)

#修改字典的key和value值
data={"A":"123","B":"456"}
data['A']="666"
print(data)

#刪除
del dict_1["d"]
dict_1

# 清除字典內的鍵keys值values
data.clear()
print(data)

# 複製字典的內容到另一字典
data={"A":"123","B":"456"}
data2=data.copy()
data2
#print(data2)
```

### 使用for loop去存取dict的資料
```
https://stackoverflow.com/questions/3294889/iterating-over-dictionaries-using-for-loops

d = {'a': 91, 'b': 72, 'c': 83} 

for key in d:
  print(key)

for k in d.keys():
    print(k)
    
for v in d.values():
    print(v)
    
for k, v in d.items():
  print(k, v)
```
### 將dict的value(key)寫成list"""
```
romanD = { "I":1,"II":2,"III":3,"IV":4,"V":5,"VI":6,"VII":7,"VIII":8,"IX":9 } 
romankeyList = [] 
romanvalueList = [] 

for key, value in romanD.items(): 
    romankeyList.append(key) 
    romanvalueList.append(value) 

#romankeyList
romanvalueList
```
### 將兩個list 合併成為一個 dictionary"""
```
romanD1 = dict(zip(romankeyList, romanvalueList))
romanD1

romanD1 = dict(zip(romanvalueList, romankeyList))
romanD1
```
### Dictionary Comprehension
```
產生一個 key為1~100的字典(dict)，value為布林值，
偶數時為True,奇數時為False
```
```
dict_even = {x:x%2==0 for x in range(1,101)}
print(dict_even)
```
### 產生a到z的ascii字典
```
ascii_a2z = {num: chr(num) for num in range(97,123)}
ascii_a2z

alphas= []
for num in range(97,123):
    alpha = chr(num)
    alphas.append(alpha)
  
ascii_a2z = {alpha: ord(alpha) for alpha in alphas}
ascii_a2z
```
### 產生ascii字典
```
ascii_dict = {num: chr(num) for num in range(256)}
ascii_dict

ascii_dict[66]
```
# [3]內建的dict函數(Dictionary Built-in Functions)
```
https://www.programiz.com/python-programming/dictionary
```
# DNA編碼
```
qiwi_infosec_ctf_2016/crypto_100_3

https://github.com/USCGA/writeups/tree/master/online_ctfs/qiwi_infosec_ctf_2016/crypto_100_3_COMPLETE
```
```
mapping = {
        
        'CGA': 'A',
        'CCA': 'B',
        'GTT': 'C',
        'TTG': 'D',
        'GGC': 'E',
        'GGT': 'F',
        'TTT': 'G',
        'CGC': 'H',
        'ATG': 'I',
        'AGT': 'J',
        'AAG': 'K',
        'TGC': 'L',
        'TCC': 'M',
        'TCT': 'N',
        'GGA': 'O',
        'GTG': 'P',
        'AAC': 'Q',
        'TCA': 'R',
        'ACG': 'S',
        'TTC': 'T',
        'CTG': 'U',
        'CCT': 'V',
        'CCG': 'W',
        'CTA': 'X',
        'AAA': 'Y',
        'CTT': 'Z',
        'ATA': ' ',
        'TCG': ',',
        'GAT': '.',
        'GCT': ':',
        'ACT': '0',
        'ACC': '1',
        'TAG': '2',
        'GCA': '3',
        'GAG': '4',
        'AGA': '5',
        'TTA': '6',
        'ACA': '7',
        'AGG': '8',
        'GCG': '9'
}

def decode_dna( string ):

    pieces = []
    for i in range( 0, len(string), 3 ):
        piece =  string[i:i+3]
        # pieces.append()
        pieces.append( mapping[piece] )

    return "".join(pieces)


string = 'GGTTCAATGGGCTTGTCAATGGTTCGCATATCCATGGGCACGGTTCGCGGCTCA'   
print(decode_dna(string))
```
