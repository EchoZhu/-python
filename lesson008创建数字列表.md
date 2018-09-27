## lesson008 创建数字列表

创建一个每个元素都是数字的列表

### range()函数
range()函数可以生成一系列数字，eg：
```python
for value in range(1,5):
    print(value)
```
range(a,b)表示生成从a到b（不包含）的一串数字，例如上述代码中，range(1,5)表示生成1,2,3,4这四个数字，不包含5。

> 那么问题来了，如果想要生成1,2,3,4,5该怎么办呢？

### 用range()函数生成列表

```python
numbers = list(range(1,6))
print(numbers)
```

> 如果想生成一个3,4,5,6,7的列表，该怎么实现呢？