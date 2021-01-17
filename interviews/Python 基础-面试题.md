### 《Python 基础》面试题

---

1. **对字典 dict={'a':24, 'g':52, 'i':12, 'k':33} 按 value 值进行排序？**

    答：sorted(dict.items(), key = lambda x:x[1])

1. **反转字符串 "hello" ？**

    &emsp;&emsp;答：print("hello"[::-1])

1. **对列表 list1 按 age 从大到小进行排序？**

    ```python
    list1 = [{'name': 'a', 'age': 20}, {'name': 'b', 'age': 30}, {'name': 'c', 'age': 25}]
    ```

    答：sorted(list1, key = lambda x:x['age'], reverse = True)

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