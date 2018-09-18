## lesson006 列表
[视频教程01](https://www.bilibili.com/video/av31499460)
[视频教程02](https://www.bilibili.com/video/av31948638)
[视频教程03](https://www.bilibili.com/video/av31950238)
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
  - 删除
    1. 删除列表中的某个元素 -> del
        ```python  
        weekday = ['Monday','Sunday','Wednesday','Thursday','Friday','Saturday']
        #第一次打印
        print(weekday)
        #删除列表中索引值为-1的元素，也就是最后一个元素'Saturday'
        del weekday[-1]
        #第二次打印，删除最后一个元素之后的列表
        print(weekday)
        #使用del 语句将值从列表中删除后，你就无法再访问它了。
        ```
      2. 弹出列表中的某个元素 -> pop
          ```python  
          weekday = ['Monday','Sunday','Wednesday','Thursday','Friday','Saturday']
          #.pop()的作用是取出列表中最后一个元素
          # 这句的操作包括两部分：1，从weekday列表中取出最后一个元素。2，把最后一个元素赋值给Saturday这个变量
          saturday = weekday.pop()
          #打印weekday列表
          print(weekday)
          #打印saturday这个变量
          print(saturday)
          # 问：当前列表中是否还有'Saturday'这个元素 ？
          # 答：没有了
          
          # .pop()默认弹出列表最后一个元素，但是可以弹出指定索引值的元素
          weekday = ['Monday','Irene','Sunday','Wednesday','Thursday','Friday']
          my_girlfriend = weekday.pop(1)
          #打印weekday列表
          print(weekday)
          #打印my_girlfriend这个变量
          print(my_girlfriend)
          ```
      > 如果你要从列表中删除一个元素，且不再以任何方式使用它，就使用del 语句;
      如果你要在删除元素后还能继续使用它，就使用方法pop() 。
      3. 根据列表某个元素的值，删除该元素 -> remove
      
      del和pop的操作都是在已知列表中需要删除的元素的索引值的情况下，当需要删除的元素的索引值未知时，可以使用remove方法
        
      ```python       
      weekday = ['Monday','Sunday','Wednesday','Thursday','Friday','Saturday']
      #第一次打印
      print(weekday)
      # 删除'Saturday'元素
      weekday.remove('Saturday')
      #第二次打印，删除最后一个元素之后的列表
      print(weekday)
      ```
     
      注意，如果需要删除的值在列表中存在多个，remove只删除第一个出现的值 
          
      ```python
      weekday = ['Saturday','Saturday','Monday','Sunday','Wednesday','Thursday','Friday','Saturday']
      #第一次打印
      print(weekday)
      # 删除'Saturday'元素
      weekday.remove('Saturday')
      #第二次打印，删除最后一个元素之后的列表
      print(weekday)
      ```
  - 组织列表
    1. 将列表中的元素进行永久排序 -> .sort()
      ```python
      alphabets = ['b','c','a','d']
      print('排序前的列表：'+str(alphabets))
      #sort方法可以改变列表中元素的按照字母表顺序排序，并且这个改变是永久性的
      alphabets.sort()
      print('排序后的列表：'+str(alphabets))
      #sort方法中传入参数：reverse=True，则可以将列表中的元素按照字母表逆序排列
      #alphabets.sort(reverse=True)
      #print('逆序排序后的列表：'+str(alphabets))
      ```
    2. 将列表中的元素进行临时排序 -> sorted
      ```python
      alphabets = ['b','c','a','d']
      print('排序前的列表：'+str(alphabets))
      #sorted（）可以临时为列表中的元素按照字母表顺序排序  
      print('排序后的列表：'+str(sorted(alphabets)))
      print('列表值：'+str(alphabets))
      ```
    3. 反转列表 -> .reverse()
      ```python
      words = ['pretty','so','is','Irene']
      print('反转前的列表：'+str(words))
      #.reverse()可永久性的反转列表中元素的排列位置
      words.reverse()
      print('反转后的列表：'+str(words))
      ```
    4. 确定列表长度
      ```python
      words = ['Irene', 'is', 'so', 'pretty']
      length = len(words)
      print('列表的长度是：'+str(length)) 
      ```   

 [回到目录](https://github.com/EchoZhu/-python/blob/master/README.md)