## 字符串类型

- 常用的数据类型，由一组字符构成，字符串用单引号或者双引号或者三个单/双引号组成。
```python
'this is a string'
"this is a string"
'''this is a string'''
"""this is a string"""
```
- 计算字符串的长度
> len(str)

```python
a = 'this is a string'
print(len(a))
'''
output:
16
'''
```

- 字符串索引和切片

字符串的下标是从0开始的，最后一位的下标为字符串的长度-1，举例：
```python
a = 'Python'

'''
 +---+---+---+---+---+---+
 | P | y | t | h | o | n |
 +---+---+---+---+---+---+
 0   1   2   3   4   5   6
-6  -5  -4  -3  -2  -1
'''
```
1. 如上面所示，字符'P'的下标为0, 则`a[0] = 'P'`，字符'n'的下标为5，则`a[5] = 'n'`, 在*python*中也可以用负数来进行索引，
表示从右开始计数，如字符'o'为从右第二个字符，则`a[-2] = 'o'` 
2. 字符串支持切片，即通过指定开始位置的下标和结束位置的下标来获取子字符串。

```python
a = 'Python'
print(a[1:2])
print(a[2:])
print(a[:3])
print(a[-2:])
print(a[:-3])
print(a[:4] + a[4:])
'''
output:
y
thon
Pyt
on
Pyt
Python
'''
```

- 分割字符串
> split(str)
```python
a = 'this is a string'
print(a.split(' ')) # 用空格分割字符串a

''''
output:
['this', 'is', 'a', 'string']
'''
```

- 判断字符串是否为某个字符串前缀
> str.startswith(xx)

```python
a = 'this is a string'
print(a.startswith('this'))

'''
output:
True
'''
```

- 判断字符串是否为某个字符串后缀
> str.endswith(xx)
```python
a = 'this is a string.'
print(a.endswith('string.'))

'''
output:
True
'''
```

- 去除指定字符串

***NOTE*** 该函数会去除收尾字符串中包含在指定字符串中的任意字符，不传参数的话默认去除空白符
> str.strip(xx)

```python
a = ' this is a string '
print('$' + a.strip(' ') + '$')
print('$' + a.strip() + '$')
print('$' + a.strip(' tg') + '$')

'''
output:
$this is a string$
$this is a string$
$his is a strin$
'''
```

- 将字符串全部变为大写
> str.upper()

```python
a = 'this is a string'
print(a.upper())

'''
output:
'THIS IS A STRING'
'''
```

- 将字符串全部变为小写
> str.lower()
```python
a = 'THIS IS A STRING'
print(a.lower())

''''
output:
'this is a string'
'''
```

- 判断子字符串是否在某个字符串中
> a.find(xx)
>
>if xx in a
>
第二种是使用`in`来判断是否在某个字符串中

```python

a = 'this is a string'
print('this' in a)
print(a.find('this'))

'''
output:
True
0 # 0表示在下标为0的地方发现'this'字符串的
'''
```


[回索引目录](type.md)