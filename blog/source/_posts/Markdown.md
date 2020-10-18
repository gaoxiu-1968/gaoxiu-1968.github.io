---
title: Markdown
date: 2020-10-17 16:07:04
tags: markdown
categories: book
---
# Markdown 

> 一种轻量级标记语言，2004年由约翰·格鲁伯（英语：John Gruber）创建

## Markdown 语法

### 标题

语法：

```txt
#
##
###
####
#####
######
共有六级标题，一级最大，六级最小
```

样例：

![image-20201010110827331](https://img-blog.csdnimg.cn/2020101716264674.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2hlaWRvbmcwMA==,size_16,color_FFFFFF,t_70#pic_center)

### 段落

> 段落没有特定的格式，段落开头可以使用制表符tab留出间隔

#### 字体

语法：

```txt
斜体：
*张明珂*

_zhangminke_

加粗：
**张明珂**

__zhangmingke__


斜体+加粗：

__*zhangmingke*__

单独使用推荐使用”*“号，在中文情况下，不用中英文切换，组合使用没有限制，推荐组合的时候_表示斜体，**表示加粗
字体的作用： 表示重点

```

样例：

![image-20201010112634348](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010112634348.png)

#### 分割线

语法：

```txt
***
___
三个星号或三个底线表示一个分割线，同行内不能有其他内容
推荐使用星号，避免中英文切换
```

样例：

![image-20201010113127749](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010113127749.png)

#### 删除线

语法：

```txt
~~张明珂~~
```

样例：

![image-20201010113327050](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010113327050.png)

#### 下划线

语法：

```html
<u>张明珂</u>
下划线是使用的html语法
```

样例：

![image-20201010113656839](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010113656839.png)

#### 脚注

> 脚注的对文本的补充说明

语法：

```txt
[^文本]: 补充说明
```

样例：

![image-20201010114310642](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010114310642.png)

### 列表

> 列表分为无序列表和有序列表

#### 无序列表

> 无序列表使用星号（*），加号（+）或者减号(在github风格下没有作用）作为列表标记，这些标记后面要跟上空格，然后写内容

语法：

```txt
* 汽车
* 摩托车
* 卡车
推荐使用*
```

样例：

![image-20201010130624386](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010130624386.png)

#### 有序列表

> 有序列表使用数字并加上.来表示，和内容要空一格

语法：

```txt
1. 汽车
2. 摩托车
3. 卡车
```

样例：

![image-20201010130924844](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010130924844.png)

#### 列表嵌套

> 在子列表的选项前添加4个空格

语法：

```txt
1. 汽车
   * 奥迪
2. 摩托车
   * 丰田
3. 卡车
   * 东风
```

样例：

![image-20201010131158214](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010131158214.png)

### 区块

> 区块引用使用在段落前，使用> 开始 空一格之后写内容 
>
> 引用： 引用是指在说话或写作中引用现成的话
>
> 现在使用的就是引用

语法：

```txt
> 引用

区块是可以嵌套的

> 最外层
> > 第一层嵌套
> > > 第二层嵌套
```

样例：

![image-20201010132014491](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010132014491.png)

### 代码

> 代码的语法一共有三种：
>
> * 表示在段落中的函数或代码行
> * 代码区块 第一种
> * 代码区块 第二种

语法：

```txt
`print()`
用反引号包围的内容表示一个函数或代码行

使用tab分割的代码块 （github主题中好像还是``` ```语法）

​```语言类型
代码
​```
语言类型可以指定也可以不指定
```

样例：

![image-20201010132836835](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010132836835.png)

### 链接

语法：

```txt
[链接名称](链接地址)

或

<链接地址>

* 符号要使用英文的才有效

高级链接：
[链接名称][链接别名]

链接别名：链接地址

不推荐使用高级链接，没什么用，解释器无法在你写的时候执行
```

样例：

![image-20201010134512006](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010134512006.png)

### 图片

语法：

```txt
![图片名](图片地址)

图片地址也可以和链接一样使用变量名替换，但是不推荐使用
```

样例：

![美女](data:image/jpeg;base64,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)

### 表格

语法：

```
|      |      |      |
| ---- | ---- | ---- |
|      |      |      |
|      |      |      |
|      |      |      |

|分割不同单元格，-分割表头和其他行

-: 设置内容和标题栏居右对齐。
:- 设置内容和标题栏居左对齐。
:-: 设置内容和标题栏居中对齐。

样例：
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |

推荐使用typora直接生成表格，易与操作！
```

样例：

![image-20201010140732743](C:\Users\SuperZhang\AppData\Roaming\Typora\typora-user-images\image-20201010140732743.png)

## Markdown高级技巧

* 和html标签混合使用
* 公式
* 流程图

一般使用不到，而且不好使用





