个人页面：qhf1430154832.github.io 
博客日记：https://blog.csdn.net/m0_53120035/article/details/117093068?spm=1001.2014.3001.5501

https://blog.csdn.net/m0_53120035/article/details/117235166
@[TOC](JavaScript 简史及基础)

## Javascript 的起源
JavaScript是由Netscape公司与sum公司（开发java语言）合作开发的。JavaScript的第一个版本1.0版本时，Netscape Navigator主宰者浏览器市场，微软为了追赶，在推出IE3的的时候发布了VBScript语言，又以JScript为名发布了JavaScript的另一个版本，面对微软公司的竞争，Netscape公司与sum公司联合ECMA（欧洲计算机制造商协会）对JavaScript进行了标准化，于是出现了ECMAScript语言，现在的JavaScript实际上就是ECMAScript。




## JavaScript的作用
1事件可以用于处理表单验证，
2.用户输入，
3.用户行为及浏览器动作:页面加载时触发事件；页面关闭时触发事件；
4.用户点击按钮执行动作；验证用户输入内容的合法性
5.网页特效制作
6.web小游戏开发










## JavaScript在HTML/XHTML文档执行方式
1.将JavaScript代码放在`<head>`标签中的`<script>`标签之间

2.将JavaScript代码作文一个以.js为扩展名的文件，再利用src属性指向该文件
`<script src"test.js"></script>`
***中间不能写入JavaScript代码***

3.将`<script>`标签放到HTML文档的最后，`</body>`标签之前

这样可以使浏览器更快的加载页面

  
# JavaScript的注释方式
我之前一直使用的注释方式为Ctrl+/来进行多行注释
//表示单行注释
/*     */注释与我之间学习的java注释方式相同。

# 变量

>变量的含义：
我们在程序中会经常定义一些变量来保存和处理数据。从本质上看，变量代表了一段可操作的内存，也可以认为变量是内存的符号化表示。
当程序需要使用内存时，可以定义某种类型的变量。此时编译器根据变量类型分配一定大小的内存空间。程序可以通过变量名来访问对应的内存；
 

 **变量名的命名规则：**
 变量和其他语法元素的名字都是区分字母大小写的，变量名允许包含字母，数字，美元符号$和下划线_（但第一个字符不允许是数字）。
 变量名中不能使用空格和标点符号（美元符号除外）。


# 数据类型
javascript语言不会像其他语言（java，c++，c...）在意变量的类型。
这种类型的语言称为弱类型语言。
1.字符串必须包含在引号里，单双引号都行。
如
```
var  name="jack"
      var name='jery'
```
2.数值 
直接赋予变量一个值，该值可以为整数和浮点数。
`var age=18`
`var money=0.0001`

3.布尔值

布尔值只有两个ture和false

# 数组
1.利用array关键字进行声明
如`var ball=Array（4）；`那么这个数组的长度就是4

2.利用小标来给数组中数值赋值
`var ball[0]="football";`
`var ball[1]="basketball"`

3.直接声明创造数组
`var ball=["football","basketball"];`

4.关联数组
在填充数组时为每一个新元素明确的给出下标来改变默认值
```
var lennon=Array();
lennon["name"]="john";
lennon["age"]=18;
lenon["living"]=false;

```
# 对象
在使用上面4.关联数组时可以把 person看作一个对象进行看待，他拥有名字，年龄，性别等属性，他也可以拥有行为如学习JavaScript，看电视，看书等行为，这种拥有属性和行为的变量可以称为对象。

对象可以用Object（）函数进行声明；
如var person=object（）；
 person.name=""
 person.age=""

简单声明
var  person={name:"",age:18,living:ture};
