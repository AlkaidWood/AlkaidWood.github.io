---
title: Markdown 标记语言常用命令
tags: Markdown
toc: ture
date: 2021-06-12 09:54:27
---

# Markdown基本语法
## 标题
添加标题：在文本前加`#`，`#`的数目代表标题的级别，最高支持六级标题
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
## 字体
斜体：`*被添加斜体的文本*`
加粗：`**被加粗文本**`
倾斜加粗：`***被倾斜加粗的文本***`
加删除线：`~~被加删除线的文本~~`
```
*被添加斜体的文本*  
**被加粗文本**
***被倾斜加粗的文本***
~~被加删除线的文本~~
```
效果演示：
    *被添加斜体的文本* 
    **被加粗文本** 
    ***被倾斜加粗的文本*** 
    ~~被加删除线的文本~~


## 分割线
在空行内输入`---`或`___`或`***`即可，符号中间也可插入空格。效果如下：

---
## 引用
在被引用的文字前加`>`
```
>这是一段引用内容，它很长很长很长很长很长很长很长------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
>
>这是第二段引用内容，它很短
```
效果如下：
>这是一段引用内容，它很长很长很长很长很长很长很长------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
>
>这是第二段引用内容，它很短

也可以控制引用的级别，`>`的个数代表级别
```
>一级文本：对于命途多舛的人生，以及渺茫的时间，阻挡在我们之间这一事实，我们无可奈何。
>>二级文本：彼方为谁，无我有问。九月露湿，待君之前。
>>>三级文本：但盼风雨来、能留你在此;即使天无雨、我亦留此地。
```
效果如下：
>一级文本：对于命途多舛的人生，以及渺茫的时间，阻挡在我们之间这一事实，我们无可奈何。
>>二级文本：彼方为谁，无我有问。九月露湿，待君之前。
>>>三级文本：但盼风雨来、能留你在此;即使天无雨、我亦留此地。
## 列表
**列表分为无序列表和有序列表。**
无序列表使用`-`或`*`或`+`进行标记，标记和文本之间要有空格，不同标记可以混用，效果相同。
```
- Harry James Potter
* Hermione Jean Granger
+ Ronald Bilius "Ron" Weasley
```
效果演示：
- Harry James Potter
* Hermione Jean Granger
+ Ronald Bilius "Ron" Weasley


有序列表使用`1.`，即任意数字加英文句号进行标记，并且数字不影响最终编译效果。
```
1. Albus Percival Wulfric Brian Dumbledore
8. Severus Snape
10. Minerva McGonagall
```
1. Albus Percival Wulfric Brian Dumbledore
8. Severus Snape
10. Minerva McGonagall

**列表可以嵌套**
在上一级与下一级列表之间敲三个空格即可。
```
* Lord Voldemort
    * Lupin
    * Dobby
        * Winky
        * Tom Riddle 
```
效果演示：
* Lord Voldemort
    * Lupin
    * Dobby
        * Winky
        * Tom Riddle 

```
1. Lord Voldemort
    1. Lupin
    1. Dobby
        1. Winky
        1. Tom Riddle 
```
效果演示：
1. Lord Voldemort
   1. Lupin
   1. Dobby
      1. Winky
      1. Tom Riddle 

**列表包含多个段落**
列表包含多个段落，每个项目下的段落都缩进4个空格或一个制表符。
```
*   Harry Potter, Protagonist, is a thin, black-haired youth wearing glasses on his forehead with a lightning-shaped scar, just as suddenly a short time overstating the children who, like flavor is not good. 
    He is a Magic School fifth-grade students, but also a man of Hogwarts. Since Voldemort after the resurrection, the scar on his forehead to his burning often endless.
```
效果演示：
*    Harry Potter, Protagonist, is a thin, black-haired youth wearing glasses on his forehead with a lightning-shaped scar, just as suddenly a short time overstating the children who, like flavor is not good. 
     He is a Magic School fifth-grade students, but also a man of Hogwarts. Since Voldemort after the resurrection, the scar on his forehead to his burning often endless.

## 代码
**在行内插入简短的代码**
把代码插入` `` `之间即可
```
看起来`codes and codes`是这样的
```
效果演示：
看起来`codes and codes`是这样的

**在行间插入代码块**
把代码块放入两行` ``` `之间(`\`是为了防止转义，实际写作中是没有的)
```
\```
start
codes and codes
end
\```
```
效果演示：
```
start
codes and codes
end
```

## 强制空行
在空行内使用`\`即可
```
第一段
\
\
第二段
```
效果演示：
第一段
\
\
第二段
