本文内容主要参考   
1·[菜鸟教程](https://www.runoob.com/markdown/md-tutorial.html)  
2·[markdown中国（可能会打不开）](http://www.markdown.cn/)    
3.[markdown台湾（国区打不开的话可以看这个繁体版）](https://markdown.tw/)

---
# 1.标题    
## 1.1.类Setext格式  
类 Setext形式是用底线形式，把=（最高>>>阶标题）和-（第二阶标题）放在内容底下一行就行  
PS：=和-放几个都行    
例如:   
```  
这是高阶标题
=
这是低阶标题
-
你可以打一片=
=========
```  
显示成这样:

这是高阶标题   
=    
这是低阶标题   
-
## 1.2类atx形式  

一级标题：# 内容（记得在#和内容中间空格）  
二级标题：## 内容；   
其他级标题类似，最多支持六级。这次得注意#的数量了哦，几个#就是几级标题 
比如：
```
##### 我是三级标题
###### 我是六级标题    
```
显示为
### 我是三级标题
###### 我是六级标题   
   
# 2段落   
## 2.1换行
Markdown 段落没有特殊的格式，直接编写文字就好，想换行的话，你可以：   
1.在本行结尾加两个以上空格加上回车  
2.在本行后面使用一个空行来表示重新开始一个段落。   
比如：   
```
这是第一行（空格）（空格）（回车）这是第二行（空格）（空格）（回车）   这是第三行（回车）
（回车）
这是第四行
```
显示为：  
这是第一行  
这是第二行   
这是第三行

这是第四行
注意，不管代码有几个空行，markdown表现出来都是只空一行，别当成word使劲敲回车，敲再多也没用，比如：  
```  
我是第一行 



我是第二行
```
显示为  
我是第一行 



我是第二行   


## 2.2字体
直接看应用   
比如：
```   
*我是斜体文本*   
_我是斜体文本_*   
*我是粗体文本**   
__我是粗体文本__     
***我是粗斜体文本***      
___我是粗斜体文本___   
```   

显示成   

*我是斜体文本*   
_我是斜体文本_*   
**我是粗体文本**   
__我是粗体文本__     
***我是粗斜体文本***      
___我是粗斜体文本___    
   
## 2.3分割线   
在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西（可以在星号或是减号中间插入空格）   
比如：
```
***   
* * *
*******
---   
- - -
___
```  

都表现表现为一毛一样的分割线   
***   
* * *
*******
---   
- - -
___   

## 2.4删除线   
在文字的两端加上两个波浪线 ~~ 即可  
比如:  
```
~~我是删除线~~
```   

表现为   
~~我是删除线~~   
## 2.5下划线   
在文本左面加```<u>```，右面加```</u>```（```/```就是斜杠，戳问号键就啦：））   
比如：
```
<u>我下面有下划线</u>
```
表现为:   
<u>我下面有下划线</u>
## 2.6脚注
比如：
```
我要写一条脚注[^脚注]
[^脚注]:脚注就是脚注啦，对某个东西进行详细说明用der
```
表现成     

我要写一条脚注[^脚注]
[^脚注]: 脚注就是脚注啦，对某个东西进行详细说明用der  

注意：GitHub的markdown（也就是你现在看到的界面）不支持脚注，因为GitHub会把脚注里面的内容当成链接（我也不知道为什么不支持emmm）。你可以看看这个有道云笔记的实例：[有道云笔记实例](http://note.youdao.com/noteshare?id=d06cb7fe6e1fa8d67b6806e749510560&sub=4908447BA1A942C28BB6438AB81402EE)  
（有一说一，虽然有道广告挺烦，但使用体验真心不错，安利一波）   
# 3列表 
## 3.1无序列表   
使用星号(*)、加号(+)或是减号(-)作为列表标记，记得在标号和内容中间空格哦
比如：
```
* 第一列
+ 第二列
- 第三列
```

表现为  
* 第一列   
+ 第二列   
- 第三列  
## 3.2有序列表  
有序列表使用数字并加上.号来表示。   
比如：
```   
1. 第一列   
2. 第二列   
```    
表现为：
1. 第一列   
2. 第二列   

## 3.3列表嵌套   
在子列表中的选项前面添加四个空格即可   
比如：
```
1. First   
    - The first
    - The second
2. Second 
    1. The first
    2. The second  
```
表现为：
1. First   
    - The first
    - The second
2. Second 
    1. The first
    2. The second   

# 4区块   
## 4.1普普通通的引用   
在段落开头使用 `>` 符号，后面+空格符号+内容   
比如：
```
>我是第一行引文   
>俺是第二行
```   
表现为：   
>我是第一行引文   
>俺是第二行   
## 4.2嵌套引用   
区块是可以嵌套的，一个`>` 符号是最外层，两个`>` 符号是第一层嵌套，以此类推：   
比如：
```
>第一层   
>>第二层   
>>>第三层
```   
表现为：   
>第一层   
>>第二层   
>>>第三层   
## 4.3 引用里嵌套列表
直接看栗子吧：   
```   
>1. first   
>2. second  
>+ emmmm   
>- emmmmmmmm   
>* emmmmmmmmmmmmmm
```     
表现为
>1. first   
>2. second  
>+ emmmm   
>- emmmmmmmm   
>* emmmmmmmmmmmmmm   

## 4.4列表里嵌套引用   
要在列表项目内放进区块，那么就需要在`>`前添加四个空格的缩进（或者一个`Tab`）   
比如：  
```   
* emmm   
1. First   
    >1. First   
    >2. Second   
2. Second   
* emmmm
```   
表现为   
* emmm   
1. First   
    >1. First   
    >2. Second   
2. Second   
* emmmm   


# 5代码   
## 5.1不需要分段的话   
用反引号（`)把要表现成代码的内容包起来   
比如：   
```
`print()    `   
```

表现为`print()`   
## 5.2需要分段的话
三个反引号开头，换行，输入内容，再换行，三个反引号结尾      
PS:可以在开头的三个反引号后，指定代码语言（当然也可以不指定）    
比如：
`````
```python   
print('Hello World!')     
```   
`````
显示为    
```python   
print('Hello World!')     
```     

# 6链接   
## 6.1链接网址   
你可以写一段文字，然后点击文字跳转到链接，也可以直接把链接放那   
```   
[链接名称](链接地址)   
<链接地址>
```
比如：   
```   
1·戳一戳[这篇文章的有道云笔记版本](http://note.youdao.com/noteshare?id=7bae46bf94336f7fccd73b5ec7ebcfc7&sub=WEB99d2250600a52cf2f920c612a800b2af)    
2·(https://github.com)   
```   
1·戳一戳[这篇文章的有道云笔记版本](http://note.youdao.com/noteshare?id=7bae46bf94336f7fccd73b5ec7ebcfc7&sub=WEB99d2250600a52cf2f920c612a800b2af)    
2·(https://github.com)   

__高级链接__  
链接链接也可以用变量来代替，文档末尾附带变量地址（本人暂时没发现这个功能有什么高级之处😶）   
比如：
```
[github][1]   

[1]:https://github.com   
```
表现为：   
[github][1]   

[1]:https://github.com 
## 6.2链接图片    
可以有以下三种方法   
```   
![](图片地址)
![属性文本](图片地址)
![属性文本](图片地址 "可选标题") 
```   
比如：   
```
![](https://raw.githubusercontent.com/whitewateroo/PicGo/master/default/2020.03.03.png)   
![示例图片](https://raw.githubusercontent.com/whitewateroo/PicGo/master/default/2020.03.03.png)   
![示例图片](https://raw.githubusercontent.com/whitewateroo/PicGo/master/default/2020.03.03.png "test")  
```
![](https://raw.githubusercontent.com/whitewateroo/PicGo/master/default/2020.03.03.png)   
![示例](https://raw.githubusercontent.com/whitewateroo/PicGo/master/default/2020.03.03.png)   
![test1](https://raw.githubusercontent.com/whitewateroo/PicGo/master/default/2020.03.03.png "test2")    
_有一说一_我觉得这仨都一样🤪
![image](https://note.youdao.com/yws/res/1874/BF63AF157DB148349E15F9467735C5EE)     

**安利**  
如上所说，你想放图片的话，得有个地方储存你的涂片，然后才能生成链接使用。这个地方就叫图床，有很多类型的图床，在这里安利一个最简单的：GitHub！   
没想到吧，通过一个免费工具Picgo即可将GitHub当作图床使用，具体操作可以参考以下内容：[GitHub搭建私人图床教程](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#github%E5%9B%BE%E5%BA%8A)
# 7表格   
用`|`分割单元格，用`-`分割表头和其他行   
比如：
```
|test1|test2|    
|---|---|   
|test3|test4|   
|test5|test6|   
|---|---|  
```

表示为：   
|test1|test2|    
|---|---|   
|test3|test4|   
|test5|test6|   
|---|---|   
你还能设置表格内容的对齐方式   
`-:`右对齐   
`:-`左对齐   
`:-:`居中对齐   
比如：
```   
|test1|test2|test2.5|    
|:----|----:|:-----:|   
|test3|test4|test4.5|   
|:-test5:|test6|test6.5|  
```     
表现为：
|test1|test2|test2.5|    
|:----|----:|:-----:|   
|test3|test4|test4.5|   
|test5|test6|test6.5|     
# 8高级操作   
## 8.1转义  
markdown里使用了很多符号表实特定意思，要是想让这些符号显示，就得转义。在markdown里，我们用反斜杠转义这些特定符号，具体操作为：一个反斜杠后面跟一个特定符号   
比如：  
```
**test**   
\*\*test\*\*
```
表现为：   
**test**   
\*\*test\*\*    

## 8.2其他  
诸如HTML、公式，我本人暂时用不到，所以没学。需要的话请回到最上面，看看我所参考的网站   
