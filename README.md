## 輸出(Input) / 輸入(Output)

### 輸入
- 語法:
```python=
input()
```
- 範例:
```python=
input() # 輸入 Hello, world!

'''
輸出結果:
'Hello, world!'
'''
```
### 輸出
- 語法:
```python=
print()
```
- 範例:
```python=
print("Hello, world!")

'''
輸出結果:
Hello, world!
'''
```
### 基本運用
- 語法:
```python=
print(input())
```
- 範例:
```python=
print(input()) # 輸入與輸出 Hello, world!

'''
輸出結果:
Hello, world!
'''
```
### 特殊用法
- 強制轉型:
```python=
int -> str # 整數 轉 字串
float -> str # 浮點數 轉 字串
str -> float # 字串 轉 浮點數
bool -> int # 布林值 轉 整數
...(更多)...
```
- 範例:
```python=
print(bool("0"))
print(float(1))
print(int(True))

'''
輸出結果:
True
1.0
1
'''
```

- 輸出格式:
    - 預設
        - 每段字串之間預設以空白分隔
        - 範例:
        ```python=
        print("Hello,", "it's me.", "Puchi")

        '''
        輸出結果:
        Hello, it's me. Puchi!
        '''
        ```   
    - sep
        - 字串之間分隔替換成其他東西
        - 範例:
        ```python=
        print("Hello,", "it's me.", "Puchi", sep="~~~")

        '''
        輸出結果:
        Hello,~~~it's me.~~~Puchi
        '''
        ```
    - end
        - 結尾的換行替換成其他東西
        - 範例:
        ```python=
        print("Hello,", "it's me.", "Puchi", end="~~~")

        '''
        輸出結果:
        Hello, it's me. Puchi~~~
        '''
        ```
    - 單引號( \' )
        - 跳脫特定字元
        - 範例:
        ```python=
        print('Hello. It\'s me.')

        """
        輸出結果:
        Hello. It's me.
        """
        ```
    - 單引號( \" )
        - 跳脫特定字元
        - 範例:
        ```python=
        print("Hello. It's \"me\".")

        """
        輸出結果:
        Hello. It's "me".
        """
        ```
    - 換行(\n) 
        - 強制換行
        - 範例:
        ```python=
        print("Hello.\nIt's me.") 

        """
        輸出結果
        Hello.                               
        It's me.
        """
        ```
    - 回車(\r)
        - 覆蓋前面字元 
        - 範例:
        ```python=
        print("Hello.\r It's me.") 

        """
        輸出結果
        It's me.
        """
        ```
    - Tab(\t)
        - 增加一個tab
        - 範例:
        ```python=
        print("Hello.\t It's me.") 

        """
        輸出結果
        Hello.	 It's me.
        """
    - BackSpace(\b) 
        - 增加一個backSpace
        - 範例:
        ```python=
        print("Hello. \b It's me.") 

        """
        輸出結果
        Hello. It's me.
        """
        ```
    - f-string
        - 範例:
        ```python=
        name = "Puchi"
        print(f"{name} says hello.")

        """
        輸出結果:
        Puchi says hello.
        """
        ```     

## 註解(Comment)
- 功用:
    - 解釋程式碼的功用
    - 增強程式的可讀性
    - 增強程式的可維護性
    - 處理不需執行的代碼段
- 語法(一):
```python=
"""
something
"""
```
- 範例:
```python=
"""
Hello, world!
"""

'''
輸出結果: 

'''
```

- 語法(二):
```python=
# something
```
- 範例:
```python=
# Hello, world!

'''
輸出結果: 

'''
```
## 型態(Type)

### 分類
| 型態 | 範例 |
| -------- | -------- |
| 整數(int)     | 0、1、123|
| 浮點數(float)     | 0.3、1.4、100.0|
| 字串(string)     |"安安"、"Puchi"、"111" |
| 布林值(bool)     |True、False |

### 查看型態
- 語法:
```python=
type()
```
- 範例:
```python=
print(type(1))

'''
輸出結果: 
<class 'int'>
'''
```

## 運算子(Operator)
### Assignment Operators
| 運算子 | 舉例 | 同等 | 意義 |
| -------- | -------- | -------- | -------- |
|**=**|x = 3|x = 3|運算等號|
|**+=**|x += 3|x = x + 3|加法|
|**-=**|x -= 3|x = x - 3|減法|
|***=**|x *= 3|x = x * 3|乘法|
|**/=**|x /= 3|x = x / 3|除法|
|**%=**|x %= 3|x = x % 3|除法取餘數|
|**//=**|x //= 3|x = x // 3|除法取商數|
|****=**|x **= 3|x = x ** 3|指數|
### Comparison Operators
| 運算子 | 意義 |
| -------- | -------- |
| **==** | 相同 |
| **!=** | 不同 |
| **>** | 大於 |
| **<** | 小於 |
| **>=** | 大於等於 |
| **<=** | 小於等於 |
### Logical Operators
| 運算子 | 意義 |
| -------- | -------- |
| **and** | 且(兩個都要符合) |
| **or**  | 或(只要一個符合) |
| **not** | 不(相反) |
### Membership Operators
| 運算子 | 意義 |
| -------- | -------- |
| **in** | 在 |
| **not in** | 不在 |
### Identity Operators
| 運算子 | 意義 |
| -------- | -------- |
| **is** | 是 |
| **not is** | 不是 |

### 比較(==、!=、=)差異

- 範例:
```python=
x = 1 # 賦予變數 x 為1
if x == 1: # 如果 x 是1
    print("It's 1.")
if x != 2: # 如果 x 不是2
    print("It's 2.")
    
"""
輸出結果:
It's 1.
It's 2.
"""
```
### 運算順序
**(由高至低排序)**
| 排序 | 運算子 | 意義 |
| -------- | -------- | -------- |
|1.|**()**|括號|
|2.|__**__|指數|
|3.| **+x, -x**	|正、負|
|4.|**, /, //, %**	|乘、除、餘數)
|5.| **+, -**|加、減|
|6.| **==, !=, >, >=, <, <=, is, is not, in, not in**|Comparison、Membership、Identity Operators|
|7.| **not**|邏輯NOT|
|8.| **and**|邏輯AND|
|9.| **or**|邏輯OR|


## 變數(Variable)
- 功用:
    - 用來儲存資料數值的容器
- 賦值
    - 將變數賦予為一種型態的值
- 變數命名規則
    1. 變數名稱的開頭必須是字母或者底線，不能以數字開頭
    2. 變數名稱只能包含字母、數字與底線
    3. 變數名稱的大小寫不一樣則被視為不同變數
    4. 不能是if, else, while等關鍵字
    5. 不要用函數名稱當變數名字

## 條件判斷(If)
- 語法:
```python=
if condition :
    do something

elif condition : 
    do something

else:
    do something
```

- 範例:
```python=
n = 2

if n < 1:
    print("It's 1.")

elif n < 2 :
    print("It's 2.")

else:
    print("It's 3.")

"""
輸出結果: 
It's 3.
"""
```

## 迴圈(Loop)
### While-Loop
- 語法:
```python=
while condition :
    do something
```
- 範例:
```python=
i = 0
while i <= 5:
    print("Hello, world!")
    i += 1

"""
輸出結果: 
Hello, world!
Hello, world!
Hello, world!
Hello, world!
Hello, world!
Hello, world!
"""
```
### For-Loop
- 語法:
```python=
for variable in iterable: 
    do something 

# Iterable（可迭代物件）: 可以一個一個輪流取出其中元素的物件
# Variable(變數): 變數是用來儲存資料數值的容器
```
- 範例:
```python=
for i in [1, 2 ,3]: 
    print(i, end = ' ')

"""
輸出結果: 
1 2 3
"""
```
- range
    - 功用:
        - 可以建立一個包含整數的iterable
    - 規則:
        - range(start, stop, step)
        - 由start至stop(不含)，每次遞增step
        - start預設是0，step預設是1
    - 範例:
    ```python=
    for i in range(5, 15, 5):
        print(i, end = ' ')

    """
    輸出結果: 
    5 10
    """
    ```
- 巢狀迴圈(Nested For)
    - 語法: 
    ```python=
    for variable_1 in iterable:
        for variable_2 in iterable:
            do something
            ...(更多)...
    ```
    - 範例:
    ```python=
    for i in range(3):
        for j in range(2):
            print(i, j)
    '''
    輸出結果: 
    0 0
    0 1
    1 0
    1 1
    2 0
    2 1
    '''
    ```
    - 規則: 外層執行n次，內層m次，則總共會執行m*n次
### Break & Continue
- break
    - 功用:
        - 跑到 break 的程式時會離開當次迴圈
    - 範例:
    ```python=
    n = 0
    while True:
        print("Hello, world!")
        n += 1
        if n == 3:
            break

    """
    輸出結果: 
    Hello, world!
    Hello, world!
    Hello, world!
    """
    ```
- continue
    - 功用:
        - 跑到 continue 的程式時會直接忽略接續程式，進入下一次迴圈
    - 範例:
    ```python=
    n = 0
    while n < 10:
        n += 1
        if (n % 2) == 0:
            continue
        print(n)

    """
    輸出結果: 
    1
    3
    5
    7
    9
    """
    ```
### While-Loop vs. For-Loop
- While-Loop
    - 有明確終止條件
    - 不確定執行次數
- For-Loop
    - 確定執行次數
    - 可用於遍歷可迭代物件

    
## 列表(List)
- 語法:
```python=
l = []
# 建立 list

len(list)
# 在 list 中有多少個項目

value in list
# 判斷 list 中的項目是否存在

list.append(value)
# 將一個新的項目加到 list 的尾端

list.extend([value_1, value_2, ...])
# 將一群接到 list 的尾端

del list[index]
# 在 list 刪除指定元素

list.insert(index, value)
# 將一個項目插入至 list 中給定的位置

list.remove(value)
# 刪除 list 中第一個值等於 x 的元素

list.pop(index)
# 移除 list 中給定位置的項目，並回傳(預設最後一項)

list.clear()
# 刪除 list 中所有項目

list.index(value, start, end)
# 回傳 list 中第一個值等於 x 的項目之索引值

list.count(value)
# 回傳 x 在 list 中所出現的次數

list.sort()
# 將 list 中的項目排序

list.reverse()
# 將 list 中的項目前後順序反過來

list.copy()
# 回傳一個複製的 list

max(list)
max(value_1, value_2, ...)
# 在 list 中最大值

min(list)
min(value_1, value_2, ...)
# 在 list 中最小值

sum(list)
# 在 list 中所有數字大小總和

sorted(list)
# 回傳一個排序好的 list

map(function, interable)
# 對 list 中的每個值都執行函式，再將所有新值放入新的 list

help(list)
# 查看詳細用法資訊
```
- 範例:
    - list
    ```python=
    l = [1, 2, 2, 3]
    print(l)

    '''
    輸出結果: 
    [1, 2, 2, 3]
    '''
    ```
    - len
    ```python=
    l = [1, 2, 2, 3]
    print(len(l))

    '''
    輸出結果: 
    4
    '''
    ```
    - in
    ```python=
    l = [1, 2, 2, 3]
    print(3 in l)
    print(4 in l)

    '''
    輸出結果: 
    True
    False
    '''
    ```
    - append
    ```python=
    l = [1, 2, 2, 3]
    l.append(4)
    print(l)

    '''
    輸出結果:
    [1, 2, 2, 3, 4]
    '''
    ```
    - del
    ```python=
    l = [1, 2, 2, 3]
    del l[3]
    print(l)

    '''
    輸出結果:
    [1, 2, 2]
    '''
    ```
    - extend
    ```python=
    l = [1, 2, 2, 3]
    l.extend([4, 5, 6])
    print(l)

    '''
    輸出結果: 
    [1, 2, 2, 3, 4, 5, 6]
    '''
    ```
    - append vs. extend
    ```python=
    l_x = [1, 2, 2, 3]
    l_y = [1, 2, 2, 3]
    l_x.append([4, 5, 6])
    l_y.extend([4, 5, 6])
    print(l_x)
    print(l_y)

    '''
    輸出結果:
    [1, 2, 2, 3, [4, 5, 6]]
    [1, 2, 2, 3, 4, 5, 6]
    '''
    ```
    - insert
    ```python=
    l = [1, 2, 2, 3]
    l.insert(1, 4)
    print(l)

    '''
    輸出結果: 
    [1, 4, 2, 2, 3]
    '''
    ```
    - remove
    ```python=
    l = [1, 2, 2, 3]
    l.remove(2)
    print(l)

    '''
    輸出結果: 
    [1, 2, 3]
    '''
    ```
    - pop
    ```python=
    l = [1, 2, 2, 3]
    l.pop(0)
    print(l)
    '''
    輸出結果:
    [2, 2, 3]
    '''
    ```
    - clear
    ```python=
    l = [1, 2, 2, 3]
    l.clear()
    print(l)

    '''
    輸出結果: 
    []
    '''
    ```
    - index
    ```python=
    l = [1, 2, 2, 3]
    print(l.index(2, 1, 3))

    '''
    輸出結果: 
    [1, 2, 2, 3]
    '''
    ```
    - count
    ```python=
    l = [1, 2, 2, 3]
    print(l.count(2))

    '''
    輸出結果: 
    2
    '''
    ```
    - sort
    ```python=
    l = [1, 2, 3, 2]
    l.sort()
    print(l)

    '''
    輸出結果:
    [1, 2, 2, 3]
    '''
    ```
    - reverse
    ```python=
    l = [1, 2, 3, 2]
    l.reverse()
    print(l)

    '''
    輸出結果:
    [3, 2, 2, 1]
    '''
    ```
    - copy
    ```python=
    l_x = [0, 1, 3, 2]
    l_y = l_x.copy()
    print(l_y[3])
    '''
    輸出結果: 
    2
    '''
    ```
    - copy比較:
    ```python=
    a = [0, 1, 3, 2]
    b = a.copy()
    c = a
    b[2] = 5
    c[2] = 7
    print(f"a = {a} \nb = {b} \nc = {c}")

    '''
    輸出結果: 
    a = [0, 1, 7, 2] 
    b = [0, 1, 5, 2] 
    c = [0, 1, 7, 2]
    '''
    ```
    - max
    ```python=
    l = [1, 2, 3, 2]
    print(max(l))
    print(max(-3, 5))

    '''
    輸出結果: 
    3
    5
    '''
    ``` 

    - min
    ```python=
    l = [1, 2, 3, 2]
    print(min(l))
    print(min(-3, 5))

    '''
    輸出結果: 
    1
    -3
    '''
    ``` 

    - sum
    ```python=
    l = [1, 2, 3, 2]
    print(sum(l))

    '''
    輸出結果: 
    8
    '''
    ``` 

    - sorted
    ```python=
    l = [1, 2, 3, 2]
    print(sorted(l))

    '''
    輸出結果: 
    [1, 2, 2, 3]
    '''
    ``` 

    - join
    ```python=
    l = ['Hello', 'world', '!']
    print(" ".join(l))

    '''
    輸出結果: 
    Hello world !
    '''
    ``` 

    - split
    ```python=
    l = "Hello world !".split(" ")
    print(l)

    '''
    輸出結果: 
    ['Hello', 'world', '!']
    '''
    ```

    - map
    ```python=
    l = [1, 2, 2, 3]
    print(list(map(str, l)))

    '''
    輸出結果: 
    ['1', '2', '2', '3']
    '''
    ```

    - help
    ```python=
    print(help("max"))

    '''
    輸出結果: 
    Help on built-in function max in module builtins:

    max(...)
    max(iterable, *[, default=obj, key=func]) -> value
    max(arg1, arg2, *args, *[, key=func]) -> value
    With a single iterable argument, return its biggest item. The
    default keyword-only argument specifies an object to return if
    the provided iterable is empty.
    With two or more arguments, return the largest argument.

    None
    '''
    ```
        
### Slicing
- 語法:
```python=
list[start: stop: step]
# 標準型

list[start: stop]
# step 預設為 1

list[start:]
# 預設至最後一項結束

list[:stop]
# 預設從第一項開始

list[:]
# 從頭到尾
```
- 範例:
```python=
l = [0, 1, 2, 3, 4, 5]
print(l[2:5:2])

'''
輸出結果: 
[2, 4]
'''
```

```python=
l = [0, 1, 2, 3, 4, 5]
print(l[2:5])

'''
輸出結果: 
[2, 3, 4]
'''
```

```python=
l = [0, 1, 2, 3, 4, 5]
print(l[2:])

'''
輸出結果: 
[2, 3, 4, 5]
'''
```

```python=
l = [0, 1, 2, 3, 4, 5]
print(l[:3])

'''
輸出結果: 
[0, 1, 2]
'''
```

```python=
l = [0, 1, 2, 3, 4, 5]
print(l[:])

'''
輸出結果: 
[0, 1, 2, 3, 4, 5]
'''
```
### Index & value
- **n [ index ]  => value**
    - 中括號裡面的數字是索引 index
    - n[index] 代表的數值是 value
- index
    - 功用: 
        - 取值
        - 修改
    - 範圍:
        - 從索引位置 "0" 開始，到索引位置 (n-1)
    - 範例:
    ```python=
    l = [1, 3, 5]
    print(l[1])
    l[1] = 7
    print(l)

    """
    輸出結果: 
    3
    [1, 7, 5]
    """
    ```
- value
    - 功用:
        - 可作為任何型態的變數
    - 範例:
    ```python=
    l = [1, 3.0, [5, 7], "Hello!"]
    print(l[1], l[2][1], l[3])

    """
    輸出結果: 
    3.0 7 Hello!
    """
    ```
### 遍歷
- 以 value 遍歷
    - 語法:
    ```python=
    for variable in iterable:
    ```
    - 範例:
    ```python=
    l = [1, 3, 5, 7]
    for i in l:
    print("value:", i)

    """
    輸出結果: 
    value: 1
    value: 3
    value: 5
    value: 7
    """
    ```
    - 規定:
        - 針對 value 做遍歷
        - 不能修改 list 本身
- 以 index 遍歷
    - 語法:
    ```python=
    for variable in range(len(iterable)):
    ```
    - 規定:
        - 針對 index 做遍歷
        - 能夠修改 list 本身
    - 範例:
    ```python=
    l = [1, 3, 5, 7]
    for i in range(len(l)):
    print("index:", i, "value:", l[i])

    """
    輸出結果: 
    value: 1
    value: 3
    value: 5
    value: 7
    """
    ```

- enumerate
    - 語法:
    ```python=
    for variable_1, variable_2 in enumerate(iterable):
    ```
    - 規定:
        - 同時對 index 和 valuey 做遍歷
    - 範例:
    ```python=
    l = [1, 3, 5, 7]
    for i, j in enumerate(l)
    print("index:", i, "value:", j)
    
    """
    輸出結果: 
    index: 0 value: 1
    index: 1 value: 3
    index: 2 value: 5
    index: 3 value: 7
    """
    ```
### funtion & method

| funtion | method |
| -------- | -------- |
|min()|append()|
|max()|insert()|
|sum()|extend()|
|map()|pop()|
|sorted()|remove()|
|split()|clear()|
|join()|count()|
|type()|index()|
|abs()|sort()|
|len()|reverse()|
|...(更多)...|...(更多)...|

## 字串(String)
- 字元
```python=
print("a") # 1 個字元
print("Hello, world!") # 多個字元組成 1 個字串

"""
輸出結果:
a
Hello, world!
"""
```
- 單行字串
    - 單引號
        - 範例:
        ```python=
        print('Hello, world!')

        """
        輸出結果:
        Hello, world!
        """
        ```
    - 雙引號
        - 範例:
        ```python=
        print("Hello, world!")

        """
        輸出結果:
        Hello, world!
        """
        ```
- 多行字串
    - 3個單引號
        - 範例:
        ```python=
        print('''Hello, world!
        Puchi''')

        """
        輸出結果:
        Hello, world!
        Puchi
        """
        ```
    - 3個雙引號
        - 範例:
        ```python=
        print("""Hello, world!
        Puchi""")

        """
        輸出結果:
        Hello, world!
        Puchi
        """
        ```
- 語法:
```python=
len(string)
# 在 string 有多少個字元

string.replace(old_value, new_value)
# 取代 string 中的字元

string.find(value, start, end)
# 尋找 string 中的字元位置

string.join(interable)
# 把一堆用 list 包起來的 string 合成一個字串

string.split(separator, maxsplit)
# 把 string 切成一堆 string 用 list 包起來
# separator: 用什麼來切，預設是空白
# maxsplit: 最多切幾次

string.strip(value)
# 刪除 string 頭尾相同的字元

string.isdigit()
# 判斷 string 中是否全為數字

string.isalpha()
# 判斷 string 中是否全為英文字母

string.isalnum()
# 判斷 string 中是否全為數字、英文字母

string.upper()
# 將 string 中的英文字母全部變成大寫

string.lower()
# 將 string 中的英文字母全部變成小寫
```
- 範例:
    - len
    ```python=
    string = "Hello, world!"
    print(len(string))

    '''
    輸出結果: 
    13
    '''
    ```

    - replace
    ```python=
    string = "Hello, world!"
    print(string.replace("world", "Puchi"))

    '''
    輸出結果: 
    Hello, Puchi!
    '''
    ```

    - find
    ```python=
    string = "Hello, world!"
    print(string.find("world"))

    '''
    輸出結果: 
    7
    '''
    ```

    - strip
    ```python=
    string = "00000Hello, world!00000"
    print(string.strip("0"))

    '''
    輸出結果: 
    Hello, world!
    '''
    ```

    - isdigit
    ```python=
    string = "78763"
    print(string.isdigit())

    '''
    輸出結果: 
    True
    '''
    ```

    - isalpha
    ```python=
    string = "Hello"
    print(string.isalpha())

    '''
    輸出結果: 
    True
    '''
    ```    

    - isalnum
    ```python=
    string = "Hello78763"
    print(string.isalnum())

    '''
    輸出結果: 
    True
    '''
    ``` 

    - upper
    ```python=
    string = "Hello, world!"
    print(string.upper())

    '''
    輸出結果: 
    HELLO, WORLD!
    '''
    ``` 

    - lower
    ```python=
    string = "Hello, world!"
    print(string.lower())

    '''
    輸出結果: 
    hello, world!
    '''
    ``` 

## 字典(Dictionay)
- 語法:
```python=
dict = {key : value}
# 建立 dictionay

len(dict)
# 在 dictionay 中有多少個項目

dict[key]
# 取值

dict.get(key)
# 搜尋 key 是否存在，否則回傳 None

dict[new_key] = new_value
# 新增

dict[old_key] = new_value
# 修改

dict.pop(key)
# 刪除指定的 key 和他對應到的 value

dict.clear()
# 刪除所有的 key 和他對應到的 value
```

- 範例:
    - dict
    ```python=
    dict = {"Bertolt" : "The Colossus Titan"}
    print(f"Bertolt is {dict['Bertolt']}.")

    '''
    輸出結果: 
    Bertolt is The Colossus Titan.
    '''
    ``` 
    
    - len
    ```python=
    dict = {"Raina" : "The Armored Titan", "Bertolt" : "The Colossus Titan"}
    print(len(dict))

    '''
    輸出結果: 
    2
    '''
    ```
    
    - 取值
    ```python=
    dict = {"Bertolt" : "The Colossus Titan"}
    print("I am", dict["Raina"]) # 取的值不存在

    '''
    輸出結果: 
    KeyError: 'Raina'
    '''
    ```
    
    - get
    ```python=
    dict = {"Bertolt" : "The Colossus Titan"}
    result = dict.get("Armin")
    print(result)

    '''
    輸出結果: 
    None
    '''
    ```

    - 新增
    ```python=
    dict = {"Bertolt" : "The Colossus Titan"}
    dict["Raina"] = "The Armored Titan" 
    print(f"I am {dict['Raina']} ,and Bertolt is {dict['Bertolt']}.")

    '''
    輸出結果: 
    I am The Armored Titan ,and Bertolt is The Colossus Titan.
    '''
    ```

    - 修改
    ```python=
    dict = {"Bertolt" : "The Colossus Titan"}
    dict["Raina"] = "The Armored Titan" 
    dict["Bertolt"] = "Eaten"
    print(f"I am {dict['Raina']} ,and Bertolt is {dict['Bertolt']}.")

    '''
    輸出結果: 
    I am The Armored Titan ,and Bertolt is eaten.
    '''
    ```
    
    - pop
    ```python=
    dict = {"Raina" : "The Armored Titan", "Bertolt" : "The Colossus Titan"}
    dict.pop("Bertolt")
    print(dict["Bertolt"]) # Bertolt 已經被刪除

    '''
    輸出結果: 
    KeyError: 'Bertolt'
    '''
    ```
    
    - clear
    ```python=
    dict = {"Raina" : "The Armored Titan", "Bertolt" : "The Colossus Titan"}
    dict.clear()
    print(dict["Raina"]) # Raina 已經被刪除

    '''
    輸出結果: 
    KeyError: 'Raina'
    '''
    ```
### 遍歷
- 以 key 遍歷
```python=
for k in dict_name.keys():
```
- 範例:
```python=
dict = {"Raina" : "The Armored Titan", "Bertolt" : "The Colossus Titan"}
for k in dict.keys():
    print(k)

'''
輸出結果: 
Raina
Bertolt
'''
```
- 以 value 遍歷
```python=
for v in dict_name.values():
```
- 範例:
```python=
dict = {"Raina" : "The Armored Titan", "Bertolt" : "The Colossus Titan"}
for v in dict.values():
    print(v)

'''
輸出結果: 
The Armored Titan
The Colossus Titan
'''
```
- 以 key, value 遍歷
```python=
for k, v in dict_name.items():
```
- 範例:
```python=
dict = {"Raina" : "The Armored Titan", "Bertolt" : "The Colossus Titan"}
for k, v in dict.items():
    print(k, v)

'''
輸出結果: 
Raina The Armored Titan
Bertolt The Colossus Titan
'''
```
### List vs. Dictionay
- list
    - 必須拿連續整數當 index
    - list[index] -> value
- dict
    - 可以拿許多不同型態當 key
    - dictionary[key] -> value


## 函式(Function)
- 語法:
```python=
def function_name(parameters): # 函數名稱
    do something # 函數內容
function_name(arguments) # 呼叫函數

# parameters(參數)
# aruments(引數)
```
- 範例:
```python=
def addition(x, y):
    print(x+y)
addition(3, 6)

"""
輸出結果: 
9
"""
```
### Id
- 功能:
    - id 回傳 Variable 存在電腦內的位置
    - "會" 改變原本數值: list, dict, set...
    - "不會" 改變原本數值: int, float, string...
- 範例:
```python=
def function_1(num): # function 內外的 int 是不同個
    num += 3

def function_2(l): # function 內外的 list 是同一個
    l += [9]

x = 2 
y = [1, 3, 5, 7] 

function_1(x)
function_2(y)

print(x)
print(y)

"""
輸出結果: 
2
[1, 3, 5, 7, 9]
"""
```
### Return
- 功能: 
    - 要讓 function 跑完可以產出一個值讓我們後續可以使用，那我們要用 function 的回傳值
- 語法:
```python=
def function_name(parameters): # 函數名稱
    do something # 函數內容
    return value # 回傳函數值
function_name(arguments) # 呼叫函數
```
- 範例:
```python=
def function(num):
    result = 1
    for i in range(1, num + 1):
        result += i
    return result
function(3)
"""
輸出結果: 
7
"""
```
### Global Variable vs. Local Variable
- 全域變數: 所有地方都能看到的變數(非函數中所宣告的變數)
- 區域變數: 只有 Function 裡面才能看到的變數(函數中宣告的變數)
- 範例:
    - 區域變數
    ```python=
    def function_1():
        x = 5 # 區域變數 x 僅能在 function_1 中使用
        y = 6
        print(x+y)

    def function_2():
        y = 1 
        print(x+y)

    function_1()
    function_2()
    
    """
    輸出結果: 
    11
    
    NameError                                 
    Traceback (most recent call last)
    Cell In[1], line 11
          8     print(x+y)
         10 function_1()
    ---> 11 function_2()

    Cell In[1], line 8
          6 def function_2():
          7     y = 1
    ----> 8     print(x+y)

    NameError: name 'x' is not defined
    """
    ```
    - 全域變數
    ```python=
    x = 5 # 全域變數 x 在 function_1、function_2 都可使用
    
    def function_1():
        y = 6         
        print(x+y)
        
    def function_2():
        y = 1
        print(x+y)    

    function_1()
    function_2()
    
    """
    輸出結果: 
    11
    6
    """
    ```

### Lambda
- 功用:
    - Lambda不需要定義名稱，並且只有一行運算式的特性，讓整體程式碼看來更加的簡潔
- 語法:
```python=
function_name = lambda parameter_1, parameter_2, ... : do something
```
- 範例:
```python=
function = lambda x, y, z : x*y*z
function(1, 3, 5)

"""
輸出結果: 
15
"""
```

## 類別(Class)
- 功能:
    - 創造一個物件
    - 把函數跟變數結合的工具
    - 可以用來建立資料結構

- 語法:
```python=
class class_name:
    pass
```

- 名詞定義:
    - method(方法)：class 裡面的 function
    - instance(實體)：依照 class 做出來的物件
    - attribute(屬性)：class 裡面的變數
- 範例:
```python=
class introduction:
def __init__(self, name, age, hobby): # method(方式)
    self.name = name # attribute(屬性)
    self.age = age
    self.hobby = hobby

About_me = introduction("Puchi", "18", "Bottle Cap Baseball") # instance(實體)
print("Name:", About_me.name)
print("Age:", About_me.age)
print("hobby:", About_me.hobby)

"""
輸出結果: 
Name: Puchi
Age: 18
hobby: Bottle Cap Baseball
"""
```
- self
    - 每個 class 中 method 的參數都要有 self
    - 決定要設定哪一個物件
    - 要用 self 才能存取 instance 中的 attribute

- __ init __
    - class 中一個的 method
    - 是一個建構子，初始化的時候用時一定要搭配 self 作為參數



### 繼承
- 功用:
    - 繼承就是以一個既有的類別，對那個類別進行擴充，變成一個新的類別
    - 原有的類別稱為"父類別"，以父類別為基礎做擴充跟改寫而成的新類別稱為"子類別"
    - 經由繼承可以降低程式的重複性
- 語法:
```python=
class (BaseClass_1, BaseClass_2, ...):
    pass
```

- super
    - 代表父類別
    - 透過 super() 執行上層 function
    - 放在 function 開頭、中間、結尾都可以
    - 單一繼承範例:
    ```python=
    class Person:
        def __init__(self, name, age):
            self.name = name
            self.age = age

    class Normalperson(Person):
        def __init__(self, name, age, punch):
            super().__init__(name, age)
            self.punch_1 = punch

    class Vampire(Person):
        def __init__(self, name, age, punch):
            super().__init__(name, age)
            self.punch_2 = punch

    Jojo = Normalperson("JOJO", "17", "olaola")
    Dio = Vampire("DIO", "120", "mudamuda")

    print("Name:", Jojo.name, "Age:", Jojo.age, "Punch:", Jojo.punch_1)
    print("Name:", Dio.name, "Age:", Dio.age, "Punch:", Dio.punch_2)

    """
    輸出結果: 
    Name: JOJO Age: 17 Punch: olaola
    Name: DIO Age: 120 Punch: mudamuda
    """
    ```
    - 多重繼承範例:
    ```python=
    class First:
        def __init__(self):
            print('First class')
            # super().__init__()  # no need


    class Second(First):
        def __init__(self):
            print('Second class')
            super().__init__()


    class Third(Second):
        def __init__(self):
            print('Third class')
            super().__init__()


    test = Third()

    """
    輸出結果: 
    Third class
    Second class
    First class
    """
    ```
    
### 參考資料
[資訊之芽 Python語法班 歷屆講義](https://github.com/tw-csie-sprout)
[Python Documentation contents](https://docs.python.org/zh-tw/3/contents.html)# Python-note
