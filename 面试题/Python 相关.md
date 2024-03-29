# 开放性问题

## 简单

1. 你是什么时候开始学 Python 的
2. 你比较常用哪个 Web 框架
3. 你觉得对你帮助最大的 Python 教程是什么，聊聊其中你印象最深的部分。
4. 你认为你学 Python 的过程中遇到的难点是什么，你现在是怎么看待这个难点的
5. 简单列举 Python 2 和 Python 3 的区别
6. Python 鸭子类型是什么意思
7. 你对 Python 中的 try except 有什么看法
8. Python 官网的地址是什么

## 一般

1. set 和 list 的区别是什么，各自的优劣和应用场景
2. type hint 是什么
3. 怎么理解 Python 的赋值语句
4. Python 函数的参数传递是怎样的

## 困难

1. 谈谈你对 Python 引用的理解，函数传递的是值传递还是引用传递，Python 有值类型吗
Python 都是引用类型，只不过有些是可变类型，有些是不可变类型，因为 Python 没有解引用（读出它的值。对它进行赋值，使它指向另一个地方。)

2. 语言 强类型 弱类型， 静态 动态的理解，Python 属于哪种
（强，动态

3. 迭代器是什么，可迭代呢？
(__next__ 函数, __iter__ 函数)

4. 了解 ORM 吗，ORM中对应数据库字段的类属性一般是怎么实现的
(描述符，运算符重载)

5. 你觉得 Web 应用中数据库链接的生命周期多长比较合适

6. Python GC 是什么，什么情况下会内存泄漏

7. 解释如下概念：class, type, instance, object, value, identity, reference, variable

## 语法问题

### 简单语法

1. "try, except, else" 和 "for else" 语句中， else 什么时候执行

2. 生成式或者推导式是什么，set, dict, list 推导式有什么区别

3. bytes 和 str 是啥，怎么转化

4. 有一个元组的列表，如何根据元组的第一个元素排序。

5. 列表切片是什么，作为左值和作为表达式有什么区别

### 困难语法

1. 描述以下语句的执行结果

```python
>>> a = (1, 2, [3, 4])
>>> a[2] += [5]

>>> True != False == True

>>> sum(10*i + j  for i in range(10) for j in range(1, 11, 1))
```

举出 4 个 magic method 就是 dunder method 说明其用途

将一个类转化为字典，你会怎么做，将一个字典转化为类呢
（参考：前者使用 key() 以及 __getitem__ 方法，后者直接使用将 mapping (asterisk) unpacking 传给类的初始化函数


__getattr__ 和 __setattr__ 是做什么的，他们的行为有什么区别
(参考，只有找不到属性时 AttributeError 才会调用 __getattr__ ，而 __setattr__ 会替换正常流程 （对应 __getattribute [əˈtrɪbjut/]


Python 类方法的本质是什么，绑定是什么意思
（参考：通过托管类访问时，函数的 __get__ 方法会返回自身的引用。但
是，通过实例访问时，函数的 __get__ 方法返回的是绑定方法对象：一种可调用的对
象，里面包装着函数，并把托管实例（例如 obj）绑定给函数的第一个参数


# 内置函数

1. 怎么对列表的各个元素求和，考虑int, str, list 以及 str, int 混合的情况。

    sum([f(i) for i in list], 0/''/[]) 

2. 怎么把 str 打印到标准错误。

    print(str, file=sys.stderr)

3. enumerate  /ɪ'numəret/  函数有什么用

4. * 怎么安全使用 eval
    
    without double underline

5. * globals, global, locals, nonlocal

6. repr  /'rɛprɪzɛn'teʃən/  和 str 的区别是什么


# 风格题

1. 如何格式化字符串，f-string 是什么
2. PEP 8 是什么



# 应用题

## 简单
1. 如何除去列表中的重复元素

2. 怎么判断一个字符串是不是 ip 地址

## 困难
1. 使用 threading 创建两个线程，如果通信？



# Web 开发

1. RESTful 有哪些含义或者说属性
