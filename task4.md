# 关键字
+关键字是python内置的，具有特殊意义的标识符，自定义标识符命名时不可与之重复。
import keyword
print(keyword.kwlist)
+ 输出：
['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']

# 函数的定义
+ 函数是封装了一些独立的功能，可以直接调用，python内置了许多函数，同时可以自建函数来使用。用 def 函数名(参数列表):  来定义，比如
def com():
      a=10
      b=20
      print(a+b)
//函数调用
定义一个函数只给了函数一个名称，指定了函数里包含的参数，和代码块结构。
这个函数的基本结构完成以后，你可以通过另一个函数调用执行，也可以直接从Python提示符执行。
# 定义函数
def printme( str ):
   "打印任何传入的字符串"
   print str;
   return;
 
# 调用函数
printme("我要调用用户自定义函数!");
printme("再次调用同一函数");

# 函数参数与作用域
  定义在函数内部的变量拥有一个局部作用域，定义在函数外的拥有全局作用域。
局部变量只能在其被声明的函数内部访问，而全局变量可以在整个程序范围内访问。调用函数时，所有在函数内声明的变量名称都将被加入到作用域中。

# 函数返回值
return语句[表达式]退出函数，选择性地向调用方返回一个表达式。不带参数值的return语句返回None。

# File
Python 提供了必要的函数和方法进行默认情况下的文件基本操作。你可以用 file 对象做大部分的文件操作。 

## 打开文件方式（读写两种方式）

open 函数 
你必须先用Python内置的open()函数打开一个文件，创建一个file对象，相关的方法才可以调用它进行读写。 
语法： 
file object = open(file_name [, access_mode][, buffering])
write()方法 
write()方法可将任何字符串写入一个打开的文件。需要重点注意的是，Python字符串可以是二进制数据，而不是仅仅是文字。 
## 文件对象的操作方法


## 学习对Excel及CSV文件进行操作
首先我们要在python环境里导入csv板块,然后我们定义一个csv文件的变量csv_file,然后通过open对此文件进行打开，打开模式采用‘r’（read：读模式）
csv文件的写入：
stu1 = ['marry',26]
stu2 = ['bob',23]
out = open('Stu_csv.csv','a', newline='')
csv_write = csv.writer(out,dialect='excel')
csv_write.writerow(stu1)
csv_write.writerow(stu2)

# Os模块
常见函数列表

os.sep:取代操作系统特定的路径分隔符
os.name:指示你正在使用的工作平台。比如对于Windows，它是'nt'，而对于Linux/Unix用户，它是'posix'。
os.getcwd:得到当前工作目录，即当前python脚本工作的目录路径。
os.getenv()和os.putenv:分别用来读取和设置环境变量
os.listdir():返回指定目录下的所有文件和目录名
os.remove(file):删除一个文件
os.stat（file）:获得文件属性
os.chmod(file):修改文件权限和时间戳
os.mkdir(name):创建目录
os.rmdir(name):删除目录

# Datetime模块
datetime模块用于是date和time模块的合集，datetime有两个常量，MAXYEAR和MINYEAR，分别是9999和1.
datetime模块定义了5个类，分别是
1.datetime.date：表示日期的类
2.datetime.datetime：表示日期时间的类
3.datetime.time：表示时间的类
4.datetime.timedelta：表示时间间隔，即两个时间点的间隔
5.datetime.tzinfo：时区的相关信息
