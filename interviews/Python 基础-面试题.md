### 《Python 基础》面试题

---

1. **对字典 dict={'a':24, 'g':52, 'i':12, 'k':33} 按 value 值进行排序？**

    &emsp;&emsp;答：sorted(dict.items(), key = lambda x:x[1])

1. **反转字符串 "hello" ？**

    &emsp;&emsp;答：print("hello"[::-1])

1. **对列表 list1 按 age 从大到小进行排序？**

    ```python
    list1 = [{'name': 'a', 'age': 20}, {'name': 'b', 'age': 30}, {'name': 'c', 'age': 25}]
    ```

    &emsp;&emsp;答：sorted(list1, key = lambda x:x['age'], reverse = True)

1. **常用的字符串格式化哪几种？**

    ```python
    name = '张三'

    # 1. 占位符
    s1 = "%s ，你好！" % name

    # 2. format
    s2 = "{} ，你好！".format(name)

    # 3. f-string
    s3 = f"{name} ，你好！"
    ```

1. **下列代码的输出是什么？**

    ```python
    list = ['a', 'b', 'c', 'd']

    print(list[10:])
    ```

    &emsp;&emsp;答：输出空列表 []

1. **用列表生成式写出公差为 11 的等差数列？**

    ```python
    print([x*11 for x in range(10)])
    ```

1. **什么是反射？**

    &emsp;&emsp;答：反射就是通过字符串的方法去访问对象的属性，调用对象的方法。

1. **简述 Python 中的深浅拷贝？**

    &emsp;&emsp;答：copy(): 浅拷贝，仅仅拷贝数据集合的第一层数据；deepcopy(): 深拷贝，拷贝数据集合的所有层。

1. **简述 Python 垃圾回收机制？**

    &emsp;&emsp;答：垃圾回收机制就是自动帮助我们管理内存，清理垃圾的一种工具。1、引用计数；2、标记-清除；3、分代回收。

1. **如何打乱列表？**

    ```python
    import random

    random.shuffle(list)
    ```

1. **Python 递归的最大层数？**

    &emsp;&emsp;答：998。

1. **什么是闭包？**

    &emsp;&emsp;答：闭包函数是指定义在函数内部的函数。内层函数可以访问外层函数的变量。

1. **实现一个装饰器，限制该函数被调用的频率，如 10 秒一次？**

    ```python
    import time

    def time_pay(func):

        def inner(*args, **kwargs):
            for line in range(10):
                print(line + 1)
                time.sleep(1)

            res = func(*args, **kwargs)

            return res

        return inner

    @time_pay
    def func1():
        print('from func1...')

    func1()
    ```

1. **Python 函数调用传参时的传递方式？**

    &emsp;&emsp;答：整数、元组和字符串这种不可变类型是值传递；列表、字典这种可变类型是引用传递。