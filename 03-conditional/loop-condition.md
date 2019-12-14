## 循环控制语句
通过for关键字或者while关键字，来控制某个代码块进行有限次或者无限次的运行。

### for 循环控制
```python
"""
对于list中的每个元素，打印出来
"""
for i in [1,2,3,4]:
    print(i) 

# output:
# 1
# 2
# 3
# 4
```

#### for x in range(n)
- **range**表示从0到n的整数（不包括n）
> range(5): [0, 1, 2, 3, 4]


### while 循环控制
```python
"""
i的初始值为0，当i一直小于6的时候，打印i，并在每一次循环结束的视乎对i进行累加。
那么i最终到6的时候就会结束循环。
"""
i = 0
while i < 6:
    print(i)
    i = i + 1
# output:
# 0
# 1
# 2
# 3
# 4
# 5

```

#### continue关键字
- 在循环体中使用，表示不执行循环体中continue一下的代码，直接进行下一次的循环
```python
for i in range(5):
    if i == 3:
        continue
    print(i)

'''
output:
0
1
2
4
'''
```

#### break关键字
- 在循环体中使用，表示直接跳出循环体。
```python
for i in range(5):
    if i == 3:
        break
    print(i)

'''
output:
0
1
2
'''
```


#### pass关键字
- 占位置的，不会改变分支路径
```python
for x in range(5):
    if x == 3:
       pass
    print(x)
'''
output:
0
1
2
3
4
'''
```

[下一节](practice.md)