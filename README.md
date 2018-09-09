# 跟小野猪一起学python
跟小野猪一起学python教学视频配套讲义。b站搜“跟小野猪一起学python”

## lesson003 字符串
1. 复习print
  - ".py" -> python解释器
  - 语法突出
2. 复习变量
  - 变量的命名规则
    - 只能是字母，数字，下划线，并且不能以数字开头
    - 不能包含空格
    - 不能与关键字重名
    - 应该具有一定的意义，具有描述性。（name is better than n）
    - 谨慎使用小写字母l和大写字母O，避免跟数字1和0重复
    - 尽量用小写
    - 多实践

3. 复习错误

4. 学习字符串
  - 字符串是由引号，包括单引号和双引号，引起来的一串字符
  - 当字符串中包含引号，要用不同引号进行区别->“‘hello‘,irene said.”
  - 将字符串第一个字母改成大写-> .title()
  - 全部改成大写.upper(),全部改成小写.lower()
  - 合并拼接字符串
  ```python 
     name = 'irene'
     print(name+' is my girlfriend.')
  ```
  - 制表符（\t）、换行符(\n)
  - 删除字符串空白.strip(), .lstrip(), .rstrip()

## lesson004 数字
1. 整数
  - 加（+ ） 减（- ） 乘（* ） 除（/ ） 运算
  - Python使用两个乘号表示乘方运算
2. 浮点数
  - 定义：Python将带小数点的数字都称为浮点数。（大多数编程语言都使用了这个术语）
  - 注意：结果包含的小数位数可能是不确定的：0.2+0.1 | 3*0.1  ，所有语言都存在这种问题，Python会尽力找到一种方式， 以尽可能精确地表示结果，就现在而言， 暂时忽略多余的小数位数即可
3. 使用函数str() 避免类型错误
  - 在将数字变量和字符串变量放在一起使用的时候要注意
   ```python 
       age = 17
       message = "I am " + age + "years old."
       print(message)
  ```
  - 复习 错误提示
  - str()
  
  ## lesson005 注释和python编程的准则
1. 注释
    - 用#表示注释的开始，井号后面的内容都会被Python解释器忽略。
    - 写注释的目的：阐述代码要做什么， 以及是如何做的。
      - 人是会遗忘的，注释帮你在很久之后重看之前写过的代码，更快的理清逻辑。
      - 以自然语言辅助代码进行说明，更容易阅读理解。
      - 与他人合作，一定要写注释，让别人更容易理解你的思路。
      - 人人都希望自己读的代码中包含注释，所以，你写代码也一定要多写简洁，清晰的注释。
      - 不用担心注释写太多，更要时刻提醒自己注释写的是不是太少了
2. python编程准则
    - 在终端输入：```import this```
    - Beautiful is better than ugly：代码可以写的很漂亮，无论是格式上还是解决问题的思路，写一段漂亮的代码，是python程序员的目标。
    - Explicit is better than implicit：显式的表达比隐晦的表示好。直接一点，用最直接的表达方式和解决问题的方式去解决问题。
      
## lesson006 列表

1. 列表：由一系列按照特定顺序排列的元素组成，在python中用[]表示列表

```python 
weekday = ['Monday','Tuesday','Wednesday','Thursday','Friday']
print(weekday)
```
2. 访问元素
  - 列表中的元素是有序排列，每个元素对应着一个索引值
  - 索引值从0开始，而不是从1开始
  - 列表中最后一个元素的索引值是-1，倒数第二个是-2
  
   ```python 
   weekday = ['Monday','Tuesday','Wednesday','Thursday','Friday']
   print(weekday[0])
   print(weekday[-1])
   ```
  - 使用列表中的某个值
     ```python 
     weekday = ['Monday','Tuesday','Wednesday','Thursday','Friday']
     today = weekday[3]
     print('Today is '+today+'.')
     ```
3. 修改、添加和删除元素
  - 列表是动态的，列表中的元素会随着程序的运行发生变化
  - 修改列表某个元素的值
     ```python 
     weekday = ['Monday','Sunday','Wednesday','Thursday','Friday']
     print('before modify weekday is \n'+str(weekday))
     weekday[1] = 'Tuesday'
     print('after modify weekday is \n'+str(weekday))
     ```
  - 向列表中增加元素,向列表末尾添加元素
     ```python 
      weekday = ['Monday','Tuesday','Wednesday','Thursday']
      print('before add Friday weekday is \n'+str(weekday))
      weekday.append('Friday')
      print('after add Friday weekday is \n'+str(weekday))
     ```
  - 向列表中增加元素,向列表中某个位置插入元素
    ```python  
      weekday = ['Monday','Tuesday','Wednesday','Friday']
      print('before insert Thursday weekday is \n'+str(weekday))
      weekday.insert(3,'Thursday')
      print('after insert Thursday weekday is \n'+str(weekday))
    
    ```
 
  





  
