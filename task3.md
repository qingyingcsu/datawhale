
# Dict字典

## 定义
+ 字典包含很多键值对，用花括号括起来。每个键值对用冒号：分割，每对之间用逗号，分割。
  键一般是唯一的，如果重复最后的一个键值对会替换前面的，值不需要唯一。值可以取任何数据类型，但键必须是不可变的，如字符串，数字或元组
## 创建
+ dict= {'a': 15, 'b': 25, 'c': 35}

## 字典的方法
包括keys、values、items、clear等方法。
+ dict.keys(), 输出：dict_keys(['a', 'b', 'c'])
+ dict.values(), 输出：dict_values([15, 25, 35])
+ dict.items(), 输出：dict_items([('a', 15), ('b', 25), ('c', 35)])
+ dict.clear(), 无输出，就是dict已被清空
cmp(dict1, dict2)  比较两个字典元素。


# 集合

## 特性
+ 用花括号定义，元素不重复，无序，因此不记录元素位置或插入点，不支持索引、切片等操作。只有键没有值

## 创建
+ s1 = {1, 2, 3, 8, 9}

## 方法
方法有add, update, pop, remove, clear等
+ s1.add(3.5), 打印s1为：{1, 2, 3, 3.5, 8, 9}
+ s1.update({2, 4, 6, 8}),打印s1为：{1, 2, 3, 3.5, 4, 6, 8}
+ s1.pop(), 返回值为：1
+ s1.remove(3), 打印s1为： {2, 3.5, 4,  6, 8}
+ s1.clear(), 无返回值，s1已清空


# 判断语句（要求掌握多条件判断）
+ 语法是：
  if 条件1：
    语句块1
  elif 条件2：
    语句块2
  else:
    语句块3
   
# 1. 定义年龄变量
age = 18

# 2. 判断是否满 18 岁
# if 语句以及缩进部分的代码是一个完整的代码块
if age >= 18:
    print("可以进网吧嗨皮……")

# 3. 思考！- 无论条件是否满足都会执行
print("这句代码什么时候执行?")

# 三目表达式
+ 输入两个数，比较它们的大小并输出其中较大者
+ print(x if(x>y) else y)
例如：
  x = input()
  y = input()
  print(x if(x>y) else y)


# 循环语句
+ for i in range(5):
    print(i)
+ 打印结果：
0
1
2
3
4
