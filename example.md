# Markdown示例

该文件用来测试和展示书写README的各种markdown语法。GitHub的markdown语法在标准的markdown语法基础上做了扩充, 称之为`GitHub Flavored Markdown`, 简称`GFM`, GFM在GitHub上有广泛应用, 除了README文件外, issues和wiki也支持markdown语法。
######　　　　　　　　　　　　　　　　　　　　　　　　　　　　　在 @guodongxiaren/README 基础上修改而得

***

## <a name="index"/>目录

* [1. 横线](#line)
* [2. 标题](#title)
* [3. 文本](#text)
    * 3.1 普通文本
    * 3.2 高亮、删除线、粗体、斜体、空格
    * 3.3 文本块
    * [3.4 块引用](#blockquotes)
* [4. 列表](#dot)
    * 4.1 圆点列表
    * 4.2 数字列表
    * 4.3 复选框列表(GFM独有)
* [5. 链接](#link)
    * 5.1 文字超链接
    * 5.2 锚点
    * [5.3 图片超链接](#piclink)
* [6. 代码](#code)
* [7. 表格](#table)
* [8. 表情](#emoji)
* [9. GFM对SM的扩展](#exptend)

## <a name="line"/>1. 横线

**\*\*\*、---、___显示虚横线, 三种效果一样**

***

---

___

PS :　___ 要与上边的文字隔一行, 否则会被认为是一、二级标题(的另一种写法), 所以用第一种就好

## <a name="title"/>2. 标题

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

PS : 一、二级标题自动带有下划线(不是虚横线)

## <a name="text"/>3. 文本

### 3.1 普通文本

这是一段普通的文本

**关于换行**

直接回车不能换行,
可以使用\<br>。 <br>
但是使用html标签就丧失了markdown的意义。可以在上一行文本后面补两个空格,  
这样下一行的文本就换行了。  
或者就是在两行文本直接加一个空行。

也能实现换行效果, 不过这个行间距有点大。

PS : 非普通文本是自动换行的

### 3.2.1 高亮

Thank `You` . Please `Call` Me `Coder`

**高亮功能也适合做一篇文章的tag**

例如:　`java` `网络编程` `Socket` `全双工`

### 3.2.2 粗体、斜体、删除线

**粗体**　　*斜体*　　~~删除线~~

**组合使用粗体、斜体、删除线:** ***斜粗体***　　***~~斜粗体删除线~~***

### 3.2.3 空格

普    通    的    空    格    多    个    只    会    显    示    为    一    个

使用全角空格, 　　全角空格被解释为汉字, 　　所以不会被被解释为HTML分隔符, 　　可以按照实际的空格数显示。

### 3.3 文本块

    欢迎到访
    很高兴见到您
    祝您, 早上好, 中午好, 下午好, 晚安

### <a name="blockquotes"/>3.4 块引用

**常用于引用文本**

文本摘自《深入理解计算机系统》P27
> **“端”(endian)的起源**  
　　令人吃惊的是, 在哪种字节顺序是合适的这个问题上, 人们表现得非常情绪化。实际上术语“little endian”(小端)和“big endian”(大端)出自Jonathan Swift的《格利佛游记》一书, 其中交战的两个派别无法就应该从哪一端打开一个半熟的鸡蛋达成一致。因此, 争论沦为关于社会政治的争论。只要选择了一种规则并且始终如一的坚持, 其实对于哪种字节排序的选择都是任意的。  
　　以下是Jonathan Swift在1726年关于大小端之争历史的描述:  
　　“……下面我要告诉你的是, Lilliput和Blefuscu这两大强国在过去36个月里一直在苦战。战争开始是由于以下的原因:我们大家都认为, 吃鸡蛋前, 原始的方法是打破鸡蛋较大的一端, 可是当今的皇帝的祖父小时候吃鸡蛋, 一次按古法打鸡蛋时碰巧将一个手指弄破了, 因此他的父亲, 当时的皇帝, 就下了一道敕令, 命令全体臣民吃鸡蛋时打破较小的一端, 违令者重罚。”  

PS : 块引用以空行结束

**块引用有多级结构**

> 数据结构
>> 树
>>> 二叉树
>>>> 平衡二叉树
>>>>> 满二叉树

## <a name="dot"/>4. 列表

### 4.1.1 圆点列表 (注意*后的空格)

* 昵称: 　阶乘！
* 别名: 　欧巴
* 英文名: Will

PS : 前后都要空行

### 4.1.2 多级圆点列表 (以4个空格为缩进)

* 编程语言
    * 脚本语言
        * Python

PS : 前后都要空行

### 4.2.1 数字列表　自动排序

可以在第一行指定`1. `(数字后面加一个点, 再加一个空格), 而接下来的几行用星号`*`就可以了, 它会自动显示成2、3、4……。

1. 封装
* 继承
* 多态

PS : 前后都要空行

### 4.2.2 多级数字列表

和圆点的列表一样, 数字列表也有多级结构, 以4个空格为缩进:

1. 这是一级的数字列表, 数字1是1
    1. 这是二级的数字列表, 阿拉伯数字在显示的时候变成了罗马数字
        1. 这是三级的数字列表, 数字在显示的时候变成了英文字母
            1. 四级的数字列表显示效果, 就不再变化了, 依旧是英文字母

PS : 前后都要空行

### 4.3 复选框列表(GFM独有)

* [x] C
* [x] C++
* [x] Qt
* [ ] C#

您可以使用这个功能来标注某个项目各项任务的完成情况, ToDoList的完成情况。

PS : 前后都要空行

## <a name="link"/>5. 链接

### 5.1 文字超链接

#### 5.1.1 链接外部URL

[我的博客](http://blog.csdn.net/lyogvce "悬停显示")　　语法 :　```[我的博客](http://blog.csdn.net/lyogvce "悬停显示")```

**另一种写法** 　语法如下:

```markdown
[我的博客][id]
[id]:http://blog.csdn.net/lyogvce "悬停显示"
```

[ ]里的id, 可以是数字, 字母等的组合。这两行可以不连着写, **一般把第二行的链接统一放在文章末尾**, id上下对应就行了。这样正文看起来会比较干净。

#### 5.1.2 链接本仓库里的URL

[emoji](./emoji.md)　　语法 :　```[emoji](./emoji.md)```

**如果文件要引用的文件不存在, 则待点击的文本为红色。引用的文件存在存在则文本为蓝色。**

### 5.2 锚点

我们可以使用HTML的锚点标签(`#`)来设置锚点 : [回到目录](#index)

### <a name="piclink"/>5.3 图片超链接

#### **显示图片**

**来源于网络的图片**　　　　　　　　　　　　　　　　　　　　　**GitHub仓库中的图片**

![baidu logo](https://www.baidu.com/img/bdlogo.gif "百度logo")　　　　![my logo](https://github.com/Will-Grindelwald/Will-Grindelwald.github.io/raw/master/profile_picture.png "我的logo")

[ ]中是图片的替代文字，图片加载失败时会显示该文字

#### **给图片加上超链接**

**第一种**　　　　　　　　　　　　　　　　　　　　　　　　　　**第二种**

[![内容任意](http://www.baidu.com/img/bdlogo.gif "点击进入百度")](http://www.baidu.com)　　　　[![head]](http://blog.csdn.net/lyogvce)
[head]: https://github.com/Will-Grindelwald/Will-Grindelwald.github.io/blob/master/profile_picture.png "点击进入我的博客"

## <a name="code"/>6. 代码

```Java
public static void main(String[]args){} // Java
```

```c
int main(int argc, char *argv[]) // C
```

```shell
echo "hello GitHub" # shell
```

```javascript
document.getElementById("myH1").innerHTML="Welcome to my Homepage"; // javascipt
```

```cpp
string &operator+(const string& A,const string& B) // cpp
```

## <a name="table"/>7. 表格

| 表头1 | 表头2 |
| ----- | ----- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| 名字 | 描述 |
| ---- | ---- |
| Help    | Display the help window.|
| Close   | Closes a window         |

**表格中也可以使用普通文本的删除线, 斜体等效果**

| 名字 | 描述 |
| ---- | ---- |
| Help    | ~~Display the~~ help window.|
| Close   | _Closes_ a window           |

**表格可以指定对齐方式**

| 左对齐 | 居中 | 右对齐 |
| :----- | :--: | -----: |
| col 3 is      | some wordy text | $1600  |
| col 2 is      |    centered     |   $12  |
| zebra stripes |    are neat     |    $1  |

**表格中嵌入图片**

| 图片 | 描述 |
| ---- | ---- |
|![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo") | baidu|

**PS : 不用对的这么齐:b**

## <a name="emoji"/>8. 表情

Github的Markdown语法支持添加emoji表情, 输入不同的符号码(两个冒号包围的字符)可以显示出不同的表情。比如`:blush:`, 可以显示:blush:。

具体每一个表情的符号码, 可以查询GitHub的官方网页[http://www.emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com)。但是这个网页每次都打开**奇慢**。。。所以@guodongxiaren整理到了[emoji](./emoji.md)中。在此感谢！

## <a name="extend"/>9. GFM对SM的扩展

1. 直接支持链接: https://www.google.com.hk (SM语法: <https://www.google.com.hk>) 见[5. 链接](#link)
* 代码块的嵌入语法不同, 见[6. 代码](#code)
