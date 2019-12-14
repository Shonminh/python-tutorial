## 条件控制语句
用来判断某个条件是否满足条件，比如判断x是否等于3，x是否是空，x+ y是否为指定的值。
### if 语句
```python
def f(x):
    print("A")
    if x == 0:
        print("B")
        print("C")
    print("D")

# f(0)
# f(1)

# output: 
# ABCD
# AD
```
### if-else 语句
```python

def f(x):
    print("A")
    if x == 0:
        print("B")
        print("C")
    else:
        print("D")
        if x == 1:
            print("E")
        else:
            print("F")
    print("G")

# f(0)
# f(1)
# f(2)
# output:
# ABCG
# ADEG
# ADFG
```

### if-else 表达式

```python
def my_abs(n):
    return n if (n >= 0) else -n

# my_abs(-5)
# my_abs(5)
# output:
# 5
# 5
```

[下一节](loop-condition.md)