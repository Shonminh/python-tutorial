## 变量
用来在程序中存储临时数据，包括全局变量和局部变量等。

### 全局变量
定义在主程序外部，可以同时被多个代码块或者程序访问。
```python
a = 'I am a global variable'
def A():
    print(a)
def B():
    print(a)

A()
B()
'''
output:
I am a global variable
I am a global variable
'''
```

### 局部变量
定义在某个代码块的内部，只能在被该代码块的作用域内被访问到。

- 函数内可访问

我们可以在不同的函数内声明相同的变量名，该变量的作用域于只限于该函数内部，不可以被外部的
函数访问到。

```python
def A():
    a = "I am a variable in A function"
    print(a)
def B():
    a = "I am a variable in B function"
    print(a)
A()
B()
'''
output:
I am a variable in A function
I am a variable in B function
'''
```

- 局部代码块内可访问

不同代码块如果其父作用域是同一个的话，那么声明的变量在该父作用域内皆可访问。
```python
def A():
    # a = "I am a variable in A function"
    for i in range(1):
        a = "I am a variable in code block1"
        print(a)
    print(a)
    for i in range(1):
        a = "I am a variable in code block2"
        print(a)
    print(a)

A()
'''output:
I am a variable in code block1
I am a variable in code block1
I am a variable in code block2
I am a variable in code block2
'''
```

### 练习

- 计算结果
```python
a = "C"
def A(a):
    print(a)
    a = "B"
    print(a)
    return a

def B(b):
    print(b)
    b = a
    print(b)

B(A("A"))
```

[回首页](../README.md)