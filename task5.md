1、类和对象
    面向对象强调对象的数据和对象的行为，一个对象包含两部分：属性（数据）和方法（函数）。
一个对象肯定属于某一个类。使用__init__定义一个类；默认值与创建指定方式混合定义。
   使用 class 语句来创建一个新类，class 之后为类的名称并以冒号结尾:
class ClassName:
   '类的帮助信息'   #类文档字符串
   class_suite  #类体
实例化类其他编程语言中一般用关键字 new，但是在 Python 中并没有这个关键字，类的实例化类似函数调用方式。
以下使用类的名称 Employee 来实例化，并通过 __init__ 方法接收参数。
"创建 Employee 类的第一个对象"
emp1 = Employee("Zara", 2000)
"创建 Employee 类的第二个对象"
emp2 = Employee("Manni", 5000)

2、正则表达式
   正则表达式是一个特殊的字符序列，它能帮助你方便的检查一个字符串是否与某种模式匹配。

3、re模块
re 模块使 Python 语言拥有全部的正则表达式功能。 
compile 函数根据一个模式字符串和可选的标志参数生成一个正则表达式对象。该对象拥有一系列方法用于正则表达式匹配和替换。 
re 模块也提供了与这些方法功能完全一致的函数，这些函数使用一个模式字符串做为它们的第一个参数。
re.match函数
re.match 尝试从字符串的起始位置匹配一个模式，如果不是起始位置匹配成功的话，match()就返回none。
函数语法：
re.match(pattern, string, flags=0)
compile 函数用于编译正则表达式，生成一个正则表达式（ Pattern ）对象，供 match() 和 search() 这两个函数使用。
语法格式为：
re.compile(pattern[, flags])

4、datetime模块学习
datatime模块重新封装了time模块，提供更多接口，提供的类有：date,time,datetime,timedelta,tzinfo。
datetime相当于date和time结合起来。
datetime.datetime (year, month, day[ , hour[ , minute[ , second[ , microsecond[ , tzinfo] ] ] ] ] )

5、http请求
我们经常会用python来进行抓包，模拟登陆等等， 势必要构造http请求包。 
http的request通常有4个方法get，post，put，delete，分别对应于查询，更新，添加，删除。我们经常用到的也就get，post。
