# markdown-tutorial
  markdown语法学习笔记

##什么是markdown
>Markdown 是一种轻量级标记语言，创始人为约翰·格鲁伯（John Gruber）。它允许人们“使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML(或者HTML)文档”。这种语言吸收了很多在电子邮件中已有的纯文本标记的特性

##markdown基本语法
###Header(标题头)
```javascript
//#号前面无空格
# H1				//在文字前面加上一个#  ，实现H1标签效果
## H2			    //在文字前面加上两个##  ，实现H2标签效果
### H3				//在文字前面加上三个###  ，实现H3标签效果
#### H4				//在文字前面加上四个####  ，实现H4标签效果
##### H5			//在文字前面加上五个#####  ，实现H5标签效果
###### H6			//在文字前面加上六个######  ，实现H6标签效果
```
__效果预览：__ 

# H1
## H2
### H3
#### H4
##### H5
###### H6


##Emphasis（强调）
###斜体（italic）
```javascript
 //在需要实现斜体效果的文字前后分别加上一个 ‘*’（星号）
 //或者一条 ‘_’(下滑线)，实现italic效果
*这个文字为斜体（italic）*
_这个文字也是斜体（italic）_
```
__效果预览：__ 

*这个文字为斜体（italic）* 
_这个文字也是斜体（italic）_ 

###粗体（blod）
```javascript
//在需要实现粗体效果的文字前后分别加上两个 ‘**’（星号）
//或者两条‘__’(下滑线)，实现blod效果
**这段文字为粗体（blod）**
__这段文字也为粗体(blod)__

```
__效果预览：__ 

**这段文字为粗体（blod）**  
__这段文字也为粗体(blod)__ 


###删除线（Strikethrough ）
```javascript
//在需要实现删除线效果的文字前后分别加上两条‘~~’（波浪线），实现
 ~~删除线效果~~
```
__效果预览：__

 ~~删除线效果~~

###文字格式混合使用
```javascript
//他们也可以合并使用
**他们也可以合并_使用_**
```
__效果预览:__

**他们也可以合并_使用_**

## Lists（列表）
###无序列表

 ```javascript
 //在要实现无须列表的文字前面加上一个‘* ’（星号加空格）
 // 或者‘+’（加号加空格）、
 //或者‘-’（减号加空格）
 //子列表前面空两格
* 列表 1
+ 列表 2
   * 列表 2-1
   - 列表 2-2
 ```
 __效果预览：__

* 列表 1
+ 列表 2
  * 列表 2-1
  - 列表 2-2

###有序列表

 ```javascript
 //在要实现有须列表的文字前面加上一个‘1.’（数字加英文的点再加空格）
 //子列表前面空两格
1. 列表 1
2. 列表 2
3. 列表 3
   * 列表 3-1
   * 列表 3-2
 ```
 __效果预览：__
 
1. 列表 1
2. 列表 2
3. 列表 3
   * 列表 3-1
   * 列表 3-2

##Links(链接)
```javascript
//直接书写链接地址，自动生成链接
1. http://github.com  or <http://www.github.com>

//内联式链接：‘[]’内部的内容表示在页面显示的内容，‘（）’表示链接地址
//[链接显示文字]（链接地址）
2. [GitHub](http://github.com)

//内联式链接，添加鼠标悬浮提示
//[链接显示文字]（链接地址  鼠标悬浮提示内容）
3. [GitHub带悬浮提示](https://www.github.com "GitHub的主页")

//参考链接有两部分组成，第一个‘[]’表示链接的文字
//第二个‘[]’表示参数名字
//在其下方要为改参数赋值,格式：[参数名]:值
4. [GitHub参考式的链接][link to GitHub] 

[link to Github]: https://www.github.com

//链接到文件相对地址，格式：[该链接显示的内容]（文件的相对路径）
5. [文件相对与该仓库的相对地址](../markdown-tutorial/master/LICENSE)

//参数链接，格式：[显示的链接名称][第几条链接]
//相对一起使用：[第几条链接]: 链接地址
6. [GitHub参数数字链接][1]

   [1]: http://github.com

  //参数链接省略参数，可以只写链接的文字内容。格式：[链接内容名称]
  //根据内容名称，对应链接地址，格式：[链接内容名称]：链接地址
7.参数链接省略参数 [GitHub参数链接省略链接名称]
	[GitHub参数链接省略链接名称]: http://www.github.com
```
__效果预览：__ 

1. http://github.com or <http://www.github.com>

2. [GitHub](http://github.com)

3. [GitHub带悬浮提示](https://www.github.com "GitHub的主页")

4. [GitHub参考式的链接][link to GitHub]

   [link to Github]: https://www.github.com

5. [文件相对与该仓库的相对地址](../markdown-tutorial/master/LICENSE)

6. [GitHub参数数字链接][1]

   [1]: http://github.org

7. 参数链接省略参数 [GitHub参数链接省略链接名称]

   [GitHub参数链接省略链接名称]: http://www.github.com

##Images（图片）
```javascript
1. Inline-style: 格式：！[不能加载图片时提示的文文字内容]（链接地址  鼠标悬停时提示的文字）
![不能加载时提示的文字](https://github.com/kenve/markdown-tutorial/blob/master/images/ecode.png?raw=true "ECode Title Text 1")

2. Reference-style: 
![不能加载时提示的文字][ECode]

[ECode]: https://github.com/kenve/markdown-tutorial/blob/master/images/ecode.png?raw=true "Logo Title Text 2"
```
__效果预览：__ 
Inline-style: 
![不能加载时提示的文字](https://github.com/kenve/markdown-tutorial/blob/master/images/ecode.png?raw=true "ECode Title Text 1") 

Reference-style: 
![不能加载时提示的文字][ECode]

[ECode]: https://github.com/kenve/markdown-tutorial/blob/master/images/ecode.png?raw=true "Ecode Title Text 2"


##引用（Blockquotes）
```javascript
//在要引用的文字前 加上‘>’大于号，前面不留空
就像XXX说的
>失败是成功之母
```
__效果预览__ 

就像XXX说的
>失败是成功之母

##代码高亮（Code and Syntax Highlighting）
```javascirpt
//单个便签不解析，用‘``’包裹
`<addr>` 便签不解析.

//代码段高亮显示
```javascript
	function fancyAlert(arg) {
 	 if(arg) {
    	$.facebox({div:'#foo'})
  }
}```

```

`<addr>` 便签不解析.





##参考资料
* 维基百科：https://zh.wikipedia.org/wiki/Markdown
* Mastering Markdown：https://guides.github.com/features/mastering-markdown/
* 