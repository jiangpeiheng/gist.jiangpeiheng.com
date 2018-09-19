# Markdown Syntax

参考:[atom Markdown help](https://www.jianshu.com/p/f3fd881548ad)  
[github Markdown help](https://help.github.com/categories/writing-on-github/)



一级标题
===

GitHub上的只是基本的语法，什么图形的那些我们在平时文字书写中使用频率太低，所以其中并没有涉及到很高的语法。
1. 基础语法：标题、字体、引用、图片、连接
2. 相对高级：代码、表格


二级标题
---

---

## 粗体/斜体/删除

*body*  
**body**  
~~delete~~  



## 引用和代码段

```
这是一段有框的文字
```

```python
def somfunc(par1='', par2=0):
  ''' docstring'''
  if par1 > par2:
    return 1
  else:
    return 0
```

> 这是引用的文字

下面是行内`有框的代码`

代码块是前面空4个空格，向pyhton[1]致敬

    python
    c++
    sudo install

## 有序和无序列表

1.
2.
3.


- 首先，要与上面的有序列表空两行以上，只空一行就会与上面的格式一致
* 然后
+ 最后
4. 之后在无序之后可以加有序表示

## 喵之图
![card](http://mmbiz.qpic.cn/mmbiz_jpg/l3Oo0icr0VH0aVicuuvCwVEZy8QjDOUBdvTWrAQUx7siclDysFY9Gnfu0wibj25aDfGcX74vm1ICCpOLJPq4mQaJbA/640?wx_fmt=jpeg&wxfrom=5&wx_lazy=1&tp=webp&wx_co=1)

Tags: 数学[y1]


## 表格支持

|项目左对齐 |价格右对齐 |数量中间对齐 |
|-------- | ---: | :----:     |
|计算机 | $1600 | 5 |

[y1]: http://www.zybuluo.com/mdeditor "yinyong"

Copyright (c) 2018 Copyright Holder All Rights Reserved.


[1]: 这是一个注脚
