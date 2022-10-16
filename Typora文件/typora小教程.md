Typora小教程

Markdown  轻量级标记语言 支持latex语法、代码高亮，自动排版

Typora删除了预览窗口，可实时预览

MarkDown的语法因不同的解析器和编辑器不同 Typora使用的是 GitHub Flavored MarkDown

#号后要有空格 

#标题  总共有6级   快捷键 ctrl+1,2.....6

#  这是一级标题

###### 这是六级标题

- 有序列表  格式 {序号}{点}{空格}{字符}
  - 快捷方式：选中需要编号的字符，Ctrl + Shift + [
  - tab 降级  shift+tab  升级
- 无序列表:*/+/-

* [ ] 任务列表:   * [ ]    



>引用： 箭头加空格    

<u>下划线</u>    ctrl+u

1. **加粗**    ctrl+b   或者 左右两个***
2. **字体倾斜   ctrl+i*
3. 回到底部  ctrl+home
4. 回到底部 ctrl+end

插入表格 ：|id|name|sex|age|

|  id  | name | sex  | age  |
| :--: | :--: | :--: | :--: |
|      |      |      |      |
|      |      |      |      |

目录：[toc]  提取所有标题

上标 <sup></sup>

ctrl + [   注销上一行格式 

### 插入图片

### ![22](C:\Users\nlp\Desktop\1.PNG)

1. 拖拽

### 插入链接及页面跳转

[百度](https:\\www.baidu.com)    

[6](#这是一级标题)

回到底部  ctrl+home

回到底部 ctrl+end

### 行间公式 ]

$$
$$ + enter
$$

 

### 插入代码块

```
三个反引号 ```
```



<h4>单元格跨行跨列:</h4>   <!--标题-->
<table border="1" width="500px" cellspacing="10">
<tr>
  <th align="left">表头(左对齐)</th>
  <th align="center">表头(居中)</th>
  <th align="right">表头(右对齐)</th>
</tr>
<tr>
  <td>行1，列1</td>
  <td>行1，列2</td>
  <td>行1，列3</td>
</tr>
<tr>
  <td colspan="2" align="center">合并行单元格</td>
  <td>行2，列3</td>
</tr>
<tr>
  <td rowspan="2" align="center">合并列单元格</td>
  <td>行3，列2</td>
  <td>行3，列3</td>
</tr>
<tr>
  <td>行4，列2</th>
  <td>行4，列2</td>
</tr>
</table>
<!--在表格td中，有两个属性控制居中显示
	align——表示左右居中——left，center，right
	valign——控制上下居中——left，center，right
	width——控制单元格宽度，单位像素
	cellspacing——单元格之间的间隔，单位像素
-->





