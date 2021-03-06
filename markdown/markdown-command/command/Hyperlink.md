## 超链接

Markdown 支持两种形式的链接语法： 行内式，参考式，还有自动链接三种形式，行内式一般使用较多。

### 3.1. 行内式

**语法说明：**

- []里写链接文字，()里写链接地址, ()中的""中可以为链接指定title属性，title属性可加可不加。title属性的效果是鼠标悬停在链接上会出现指定的 title文字。[链接文字](链接地址 "链接标题")这样的形式。***链接地址与链接标题前有一个空格。\***

**代码：**

```cpp
欢迎来到[github](http://www.github.com)
```
**显示效果：**
 欢迎来到[github](https://www.github.com)

### 3.2. 参考式

参考式超链接一般用在学术论文上面，或者另一种情况，如果某一个链接在文章中多处使用，那么使用引用 的方式创建链接将非常好，它可以让你对链接进行统一的管理。

**语法说明：**
 参考式链接分为两部分，文中的写法 [链接文字][链接标记]，在文本的任意位置添加[链接标记]:链接地址 "链接标题"，***链接地址与链接标题前有一个空格。\***

如果链接文字本身可以做为链接标记，你也可以写成[链接文字][]
 [链接文字]：链接地址的形式，见代码的最后一行。

**代码：**
```ruby
我经常去的几个网站[GitHub][1]、[知乎][2]以及[简书][3]
[简书][3]是一个不错的[写作社区][]。

[1]:https://github.com "GitHub"
[2]:https://www.zhihu.com "知乎"
[3]:http://www.jianshu.com "简书"
[写作社区]:http://www.jianshu.com
```

**显示效果：**
 我经常去的几个网站[GitHub](https://github.com)、[知乎](https://www.zhihu.com)以及[简书](https://www.jianshu.com)
 [简书](https://www.jianshu.com)是一个不错的[写作社区](https://www.jianshu.com)。

### 3.3. 自动链接

**语法说明：**
 Markdown 支持以比较简短的自动链接形式来处理网址和电子邮件信箱，只要是用<>;包起来， Markdown 就会自动把它转成链接。一般网址的链接文字就和链接地址一样，例如：

**代码：**

```dart
<http://example.com/>
<address@example.com>
```

**显示效果：**
 http://example.com/
 [address@example.com](mailto:address@example.com)

