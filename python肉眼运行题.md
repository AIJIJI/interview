# 题目

分别描述以下语句的执行结果

1. 难

```python
>>> a = (1, 2, [3, 4])
>>> a[2] += [5]
```

2. 难

```python
>>> True != False == True
```

3. 简单

```python
>>> sum(
    10*i + j
    for i in range(10)
    for j in range(1, 11, 1))
```

4. 难

```python
>>> b = 9
>>> def f():
...     print(b)
...     b = 3
...
>>> f()
```

5. 极难

```python
>>> from copy import copy
>>> a = (1, 2)
>>> (1,2) == copy(a) is a



# 答案与解析

1. 

(1, 2, [3, 4, 5])  5分
报错 5分
考点：tuple list

2. 

False
考点：比较

3. 
5050

4.
UnboundLocalError: local variable 'b' referenced before assignment
考点：作用域