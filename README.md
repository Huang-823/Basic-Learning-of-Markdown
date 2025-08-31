# <center> Markdown基础语法</center>  

## 一.标题  

- 两种标题形式：
  
### 1）使用`=`和`-`标记一级和二级标签  

>一级标题  
>`=====`  
>二级标题  
>`-----`  

效果：  

> 一级标题
>=====  
>
>二级标题
>-----  

### 2）使用`#`表示1-6级标题  

>\# 一级标题  
>\## 二级标题  
>\### 三级标题  
>\#### 四级标题  
>\##### 五级标题  
>\###### 六级标题  

效果：  

># 一级标题
>
>## 二级标题
>
>### 三级标题
>
>#### 四级标题
>
>##### 五级标题
>
>###### 六级标题  

## 二.段落  

段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用**两个以上**空格加上回车（引用中换行省略回车）。  

## 三.区块引用  

在段落的每行或者只在第一行使用`>`,还可以多个嵌套使用：  
>\>区块引用  
>\>>嵌套引用  

效果：  

>区块引用  
>>嵌套引用  

## 四.代码区块  

### 1）使用` ``` `加上编程语言进行代码区块的书写  

> \```python
> print(
>   hello Markdown
> )
> \```  

效果：  

```python
print(
    Hello Markdown
)
```  

### 2）每行加上4个空格或者一个制表符（如同写代码一样）  

代码区块：

    void main()
    {
        printf("Hello, Markdown.");
    }

==**注意**:需要和普通段落之间存在空行。==  

## 五.文本内容  

### 1）字体  

|字体|代码|
|:--:|:--:|
|*斜体*|* *|
|*斜体*|__|
|**粗体**|** **|
|**粗体**|____|
|***粗斜体***|*** ***|
|==高亮==|== ==|
|~~删除~~|~~ ~~|
|<u>下划线</u>|`<u> </u>`|

### 2）链接  

链接可以由两种形式生成：**行内式**和**参考式**.  

**行内式**：  
>\[外刊Nature网址](<https://www.nature.com/>)  

效果：
>[外刊Nature网址](https://www.nature.com/)  

**参考式**：
> \[外刊Nature网址]\[1]  
>......  
> \[1]: <https://www.nature.com/>  

效果：  
>[外刊Nature网址][1]  
>......  
>[1]:https://www.nature.com/  

### 2）列表  

**有序列表：**  
有序列表的标记方式是将上述的符号换成数字,并辅以`.`，如：  

1. 列表一
   1. 列表一
        1. 列表一
        2. 列表二
        3. 列表三
   2. 列表二
   3. 列表三
2. 列表二
3. 列表三  

**无序列表：**  
使用`·`、`+`、或`-`标记无序列表，如：  

- 列表一
- 列表二
- 列表三  

### 3）脚注  

>什么是Nature\[^1]

效果：  
>什么是Nature[^1]

## 六.图片  

**1）使用markdown语法插入：**  
*添加图片的形式和链接相似，只需在链接的基础上前方加一个`！`。*  

`![Boy.jpg](https://github.com/Huang-823/Basic-Learning-of-Markdown/blob/main/FILE/Boy.jpg)`  

![Boy.jpg](https://github.com/Huang-823/Basic-Learning-of-Markdown/blob/main/FILE/Boy.jpg)  

**2）使用图床插入：**  
上传图片至[图床](https://imgse.com/)，会获得一个markdown地址，粘贴在md文档里即可查看。例如：  

`[![pELYCZD.md.jpg](https://s21.ax1x.com/2025/05/07/pELYCZD.md.jpg)](https://imgse.com/i/pELYCZD)`  

[![pELYCZD.md.jpg](https://s21.ax1x.com/2025/05/07/pELYCZD.md.jpg)](https://imgse.com/i/pELYCZD)

**3）使用HTML修改图片格式**  
原图HTML代码：
`<a href="https://imgse.com/i/pELYCZD"><img src="https://s21.ax1x.com/2025/05/07/pELYCZD.jpg" alt="pELYCZD.jpg" border="0" /></a>`  

将图片宽度调为50%并居中效果：  
`<a href="https://imgse.com/i/pELYCZD"><div align=center><img src="https://s21.ax1x.com/2025/05/07/pELYCZD.jpg" alt="pELYCZD.jpg" border="0" width="50%"/></div></a>`  

<a href="https://imgse.com/i/pELYCZD"><div align=center><img src="https://s21.ax1x.com/2025/05/07/pELYCZD.jpg" alt="pELYCZD.jpg" border="0" width="50%"/></div></a>

## 七.Todolist  

> \- [x] 事项一  
> \- [ ] 事项二  
> \- [ ] 事项三   

效果：  

> - [x] 事项一
> - [ ] 事项二
> - [ ] 事项三  

## 八.表格  

|左对齐|居中对齐|右对齐|
|:----|:----:|-----:|
|a|b|c|
|语法形式|语法形式|语法形式|
|`:---`|`:---:`|`---:`|  

## 九.分割线  

单独使用三个`*`，表示分割线  

示例：  
***

## 十.插入latex数学公式  

**行内显示：**
> 这是一个数学公式：\$f(x)=ax+b$

效果：
> 这是一个数学公式：$f(x)=ax+b$

**块内显示数学表达式：**
>
> ```
> $$
> \begin{Bmatrix}
> a & b \\
> c & d
> \end{Bmatrix}
> $$
> ```

效果：
> $$
> \begin{Bmatrix}
> a & b \\
> c & d
> \end{Bmatrix}
> $$

## 十一.HTML和CSS语法美化文档  

**HTML**  
> \<center>\<font face="仿宋" size=5>我爱学Python\</font>\</center>
> \<font face="华文楷体" font color=green>Markdown是一类好用的轻量化语言\</font>

效果：  
> <center><font face="仿宋" size=5>我爱学Python</font></center>
> <font face="华文楷体" font color=green>Markdown是一类好用的轻量化语言</font>

**CSS**  
**ctrl+shift+P**搜索"**Markdown Preview Enhanced:Customize CSS**"在**style**中使用CSS语法改标点格式等  

打开如下：  

```css
/* Please visit the URL below for more information: */
/*   https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css */

.markdown-preview.markdown-preview {
  // modify your style here
  // eg: background-color: blue;
}
```  

修改一级，二级标题颜色为红色：  

```css
/* Please visit the URL below for more information: */
/*   https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css */

.markdown-preview.markdown-preview {
  // modify your style here
  // eg: background-color: blue;
  h1,h2{
    color: #e90f0f;
  }
}
```

## 十二.PDF导出  

**1）使用 Markdown PDF 导出**（不推荐）  

**2）右键预览文件，点击 Open in Browser，在浏览器中右键选择打印，选择PDF格式导出即可**  

[^1]:Nature是一个外刊网站
