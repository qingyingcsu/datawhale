
# 环境搭建
## anaconda环境配置
+ 这部分直接安装anaconda即可，我安装的版本是 “Anaconda3-4.5.12-Windows-x86_64.exe”，对应的python版本是3.6.8

## 解释器
ipython交互式解释器，也称为shell.

# python初体验
## print and input
- python3的print作为一个函数，必须用 print("你要打印的字符串")这样的格式表达，即要打印的东西要用括号括起来
- input是使用键盘输入，输入的内容会被认为是一个字符串，要用一个变量来接受，例如 b = input("please input a number: ")。从键盘输入
的字符串还可以强制转换成其他数据类型。

# python基础讲解
## python变量特性+命名规则
+ 
变量用来存储数据。变量名的长度不受限制，但其中的字符必须是字母、数字、或者下划线（_），而不能使用空格、连字符、标点符号、引号或其他字符。
+ 变量名的第一个字符不能是数字，而必须是字母或下划线。
+ Python区分大小写。
+ 不能将Python关键字用作变量名。

## 注释方法
两种注释方法：
+ 单行注释以 # 开头，例如：

  /# 某个注释
+ 多行注释用三个单引号 ''' 或者三个双引号 """ 将注释括起来，例如:

  '''
  
  这是多行注释，用三个单引号
  
  '''
  
  或者
  
  """
  
  这是多行注释，用三个双引号
  
  """
  

## python中“：”作用
冒号“:”的作用是取数据，含左不含右，如果冒号左右都留空，则取所有
例如 X[:, m:n]表示取矩阵X所有行中的m到n-1列


## 学会使用dir( )及和help( )

+python内置了很多内置函数、类方法属性及各种模块。当我们想要当我们想要了解某种类型有哪些属性方法以及每种方法该怎么使用时，我们可以使用dir()函数和help()函数在python ide交互式模式下获得我们想要的信息。 dir() 函数不带参数时，返回当前范围内的变量、方法和定义的类型列表；带参数时，返回参数的属性、方法列表。如果参数包含方法__dir__()，该方法将被调用。如果参数不包含__dir__()，该方法将最大限度地收集参数信息。dir() 函数不带参数时，返回当前范围内的变量、方法和定义的类型列表，
例如 dir()，返回

  ['__annotations__', '__builtins__', '__doc__', '__loader__', '__name__', '__pac
age__', '__spec__', 'a', 'b']

+ dir(b)，返回

  ['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '_
_eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs
__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__iter__', '__le__'
, '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__',
'__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__'
, '__str__', '__subclasshook__', 'capitalize', 'casefold', 'center', 'count', 'e
ncode', 'endswith', 'expandtabs', 'find', 'format', 'format_map', 'index', 'isal
num', 'isalpha', 'isdecimal', 'isdigit', 'isidentifier', 'islower', 'isnumeric',
 'isprintable', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstr
ip', 'maketrans', 'partition', 'replace', 'rfind', 'rindex', 'rjust', 'rpartitio
n', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase'
, 'title', 'translate', 'upper', 'zfill']


+ help()是帮助函数
  例如 help(print)，会输出：
  Help on built-in function print in module builtins:

  print(...)
    print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)

    Prints the values to a stream, or to sys.stdout by default.
    Optional keyword arguments:
    file:  a file-like object (stream); defaults to the current sys.stdout.
    sep:   string inserted between values, default a space.
    end:   string appended after the last value, default a newline.
    flush: whether to forcibly flush the stream.
    
## import使用
  import ***  的作用是导入外部模块，例如
  import numpy as np
  python中有些库是内置库，有些第三库需要单独安装。

## pep8介绍
  pep8实际上是要写出优雅代码的一些格式规范和命名规则，像缩进、空行等等。需要在实际的代码编写过程中熟悉和掌握。


# python数值基本知识
## python中数值类型，int，float，bool，e记法等

整数类型（int）简称整型，它用来表示整数，例如 100、212等。代码 a=100
浮点型（float）用于表示实数，例如3.14、9.5。代码 b=3.14
布尔型只能是True和Flase，例如：None,[],()等都是Flase。
复数类型用于表示数学里的复数，例如：c=5+2j,c.real就是5.0，c.imag就是2.0。  


## 逻辑运算符
逻辑运算符用来表示“并且”“或者”“除非”等思想。and布尔“与”，or布尔“或”，not布尔“非”


## 成员运算符

成员运算符in \ not in用来判断指定序列中是否包含某个值，如果包含，返回Ture,否则返回Flase。
## 身份运算符

is 是判断两个标识符是不是引用同一个对象，	is not 是判断两个标识符是不是引用不同对象。
is 与 == 区别：
is 用于判断 两个变量 引用对象是否为同一个。== 用于判断 引用变量的值 是否相等
## 运算符优先级
如果某个表达式中同时使用了多个运算符，这些运算符的优先级是不同的。**指数是最高优先级，其次分别为为按位翻转~，一元加号和减号，
* / % // + — >>  <<  & ,再次为比较运算符、等于运算符、赋值运算符、成员运算符、逻辑运算符。
