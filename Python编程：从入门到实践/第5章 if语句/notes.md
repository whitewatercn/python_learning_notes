## 5.2条件测试  
每条if语句都是一个值为True或False的表达式（即条件表达式），根据是True还是False决定是否执行if语句中的代码  
### 5.2.2检查是否相等   
相等运算符`==`，用于发问：前面这个和后面这个相同吗？若相同，返回True，否则False   
* 一般情况下，检查时要注意大小写  
```   
>>>car = 'Audi'   
>>>car == 'audi'   
False   
```   
* 要是不在意大小写区别的话，可以把变量转换成小写再进行比较   
```   
>>>car = 'Audi'   
>>>car.lower() == 'audi'  
True
```  
PS：lower()不会修改变量car，只是比较时处理而已   
### 5.2.3检查是否不相等   
```
>>>requested_topping = 'mushrooms'  
>>>if requested_topping != 'anchovies':
>>>    print("Hold the anchovies!")
Hold the anchovies!
```   
### 5.2.4比较数字   
* 检查相等或不相等，和前面一样
```
>>>age = 18
>>>age ==18
True
```   
* 比较大小（小于、小于等于、大于、大于等于）   
```
>>> age = 19
>>> age < 21
True
>>> age <= 21
True
>>> age > 21
False
>>> age >= 21
Flase   
```   
### 5.2.5检查多个条件   
1. and   
两个条件都符合，返回True，否则False   
```
>>> age_0 = 22  
>>> age_1 = 18
>>> age_0 >=21 and age_1>=21
False
>>> age_1 = 22
>>> age_0 >= 21 and age_1 >=21 
True
```   
为了好看，将测试内容放在圆括号里头   
```
(age_0 >= 21) and (age_1 >=21) 
```   
2. or  
至少有一个条件符合，返回True，否则False  
```
>>> age_0 = 22  
>>> age_1 = 18
>>> age_0 >=21 or age_1>=21
True
>>> age_0 = 18
>>> age_0 >= 21 and age_1 >=21 
False
```   
### 5.2.6检查特定值是否包含在列表中  
```
>>> colors = ['red','whtie','black']
>>> 'yellow' in colors
Flase
>>> 'red' in colors 
True  
``` 
### 5.2.7检查特定值是否不包含在列表中  
```
>>> colors = ['red','whtie','black']
>>> 'yellow' not in colors
True
>>> 'red' not in colors 
False 
```   
### 5.2.8布尔表达式     
还是条件表达式
