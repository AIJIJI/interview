# 开放性问题

## 简单
1. 你是什么时候开始学 Python 的 
2. 你比较常用哪个 Web 框架
3. 你觉得对你帮助最大的 Python 教程是什么，聊聊其中你印象最深的部分。
4. 你认为你学 Python 的过程中遇到的难点是什么，你现在是怎么看待这个难点的
5. 简单列举 Python 2 和 Python 3 的区别
6. Python 鸭子类型是什么意思
7. 你对 Python 中的 try except 有什么看法


## 困难
1. 谈谈你对 Python 引用的理解，函数传递的是值传递还是引用传递，Python 有值类型吗
Python 都是引用类型，只不过有些是可变类型，有些是不可变类型，因为 Python 没有解引用（读出它的值。对它进行赋值，使它指向另一个地方。)

2. 语言 强类型 弱类型， 静态 动态的理解，Python 属于哪种
（强，动态

3. 迭代器是什么，可迭代呢？
(__next__ 函数, __iter__ 函数)

4. 了解 ORM 吗，ORM中对应数据库字段的类属性一般是怎么实现的
(描述符，运算符重载)

5.你觉得 Web 应用中数据库链接的生命周期多长比较合适


简单语法：
列表生成式是什么？
bytes 和 str 是啥，怎么转化


困难技巧：
举出 4 个 magic method 就是 dunder method 说明其用途

将一个类转化为字典，你会怎么做，将一个字典转化为类呢
（参考：前者使用 key() 以及 __getitem__ 方法，后者直接使用将 mapping (asterisk) unpacking 传给类的初始化函数


__getattr__ 和 __setattr__ 是做什么的，他们的行为有什么区别
(参考，只有找不到属性时 AttributeError 才会调用 __getattr__ ，而 __setattr__ 会替换正常流程 （对应 __getattribute [əˈtrɪbjut/]


Python 类方法的本质是什么，绑定是什么意思
（参考：通过托管类访问时，函数的 __get__ 方法会返回自身的引用。但
是，通过实例访问时，函数的 __get__ 方法返回的是绑定方法对象：一种可调用的对
象，里面包装着函数，并把托管实例（例如 obj）绑定给函数的第一个参数


你的职位是运维开发，求值意向是 Python 开发工程师，为什么



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

