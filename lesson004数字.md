## lesson004 数字
[视频教程](https://www.bilibili.com/video/av31351569?_blank)
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

  [下一课](https://github.com/EchoZhu/-python/blob/master/lesson005注释和python编程的准则.md)

  [回到目录](https://github.com/EchoZhu/-python/blob/master/README.md)