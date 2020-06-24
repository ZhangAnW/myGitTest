# Markdown简介

[toc]

- [ ] 

- [x] 





Markdown是一种纯文本格式的标记语言。通过简单的标记语法，它可以使普通文本内容具有一定的格式。
相比WYSIWYG编辑器

> typora
>
>  显示侧边栏CTRL +SHIFT + L
>
> 显示源代码 CTRL + /
>
> 搜索 CTRL +SHIFT + F



## 优点：（CTRL + 2）



>1、因为是纯文本，所以只要支持Markdown的地方都能获得一样的编辑效果，可以让作者摆脱排版的困扰，专心写作。
>
>2、操作简单。比如:WYSIWYG编辑时标记个标题，先选中内容，再点击导航栏的标题按钮，选择几级标题。要三个步骤。而Markdown只需要在标题内容前加#即可



## 缺点：（CTRL + 2）

>1、需要记一些语法（当然，是很简单。五分钟学会）。
>
>2、有些平台不支持Markdown编辑模式。



## 一、标题
在想要设置为标题的文字前面加#来表示
一个#是一级标题，二个#是二级标题，以此类推。支持六级标题。

注：标准语法一般在#后跟个空格再写文字，貌似简书不加空格也行。

## 二、 文件格式

==我高亮了==

**这是加粗的文字** CTRL + B

*这是倾斜的文字*` CTRL + I

***这是斜体加粗的文字***

~~这是加删除线的文字~~ ALT + SHIFT + 5

<u> 这是下划线</u> ctrl+u


>这是引用的内容
>
>
>>这是引用的内容
>>
>>>>>>>>>>这是引用的内容(可以嵌套)

分割线


三个或者三个以上的 - 或者 * 都可以。

---
----
***
*****

>上下标2^2^ H~2~o

## 图片
语法：

![数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark](数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark '描述信息')

![数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark](\Users\nick\mac\desktop\数据类型总结-搞笑结束.jpg?x-oss-process=style/watermark '描述信息')
![图片alt](图片地址 ''图片title'')

图片alt就是显示在图片下面的文字，相当于对图片内容的解释。
图片title是图片的标题，当鼠标移到图片上时显示的内容。title可加可不加
示例：

![blockchain](https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/
u=702257389,1274025419&fm=27&gp=0.jpg "区块链")

上传本地图片直接点击导航栏的图片标志，选择图片即可

## 超链接

语法：

>[超链接名](超链接地址 "超链接title")
title可加可不加
###示例：

[简书](http://jianshu.com)

[百度](http://baidu.com)

>注：Markdown本身语法不支持链接在新页面中打开，貌似简书做了处理，是可以的。别的平台可能就不行了，如果想要在新页面中打开的话可以用html语言的a标签代替。
>
<a href="超链接地址" target="_blank">超链接名</a>
>
>示例
><a href="https://www.jianshu.com/u/1f5ac0cf6a8b" target="_blank">简书</a>



## 列表
### 无序列表
#### 语法：

无序列表用 - + * 任何一种都可以 ctrl + shift +]

- 列表内容

+ 列表内容
* 列表内容

注意：- + * 跟内容之间都要有一个空格

### 有序列表
#### 语法：

数字加点

1. 列表内容
2. 列表内容
3. 列表内容

>注意：序号跟内容之间要有空格

## 列表嵌套

> Tab键

+ 一级无序列表内容    
  +  二级无序列表内容
  + 二级无序列表内容
    + 三级无序列表内容
 - 一级无序列表内容
    - 二级有序列表内容
    - 二级有序列表内容
    - 二级有序列表内容
- 一级有序列表内容
   - 二级无序列表内容
   - 二级无序列表内容
   - 二级无序列表内容
 - 一级有序列表内容
    - 二级有序列表内容
    - 二级有序列表内容
    - 二级有序列表内容

## 表格（CTRL+T）

表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

> 第二行分割表头和内容。
> - 有一个就行，为了对齐，多加了几个
> 文字默认居左
> -两边加：表示文字居中
> -右边加：表示文字居右
> 注：原生的语法两边都要用 | 包起来。此处省略

姓名|技能|排行
--|:--:|--:
刘备|哭|大哥
关羽|打|二哥
张飞|骂|三弟
## 代码

### 单行代码：代码之间分别用一个反引号包起来

​    `代码内容`
​    

### 代码块：代码之间分别用三个反引号包起来，且两边的反引号单独占一行

```
  代码...
  代码...
  代码...
```

`create database hero;`

```
    function fun(){
         echo "这是一句非常牛逼的代码";
    }
    fun();
```
## 流程图

```flow
st=>start: 开始
op=>operation: My Operation
cond=>condition: Yes or No?
e=>end
st->op->cond
cond(yes)->e
cond(no)->op
```
## 内嵌数学公式 

$\sum_{i=1}^{10}f(i)\,\,\text{thanks}$
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$
:sleeping:

## 注脚

使用 Markdown[^1]可以效率的书写文档, 直接转换成 HTML[^2]

[^1]:Markdown是一种纯文本标记语言

[^2]: 我也不知道注释啥 



<!--zhu shi-->



>链接：https://www.jianshu.com/p/191d1e21f7ed
>
>来源：简书