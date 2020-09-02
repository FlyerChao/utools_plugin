## 插入图像

图片的创建方式与超链接相似，而且和超链接一样也有两种写法，行内式和参考式写法。

语法中图片Alt的意思是如果图片因为某些原因不能显示，就用定义的图片Alt文字来代替图片。 图片Title则和链接中的Title一样，表示鼠标悬停与图片上时出现的文字。 Alt 和 Title 都不是必须的，可以省略，但建议写上。

### 7.1. 行内式

**语法说明：** ![图片Alt](图片地址 "图片Title")

**代码：**



```ruby
快乐学习： 
![快乐学习](http://upload-images.jianshu.io/upload_images/1001659-7535c9e3fe16240d?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "快乐学习")
```

**显示效果：**

快乐学习：



![img](https:////upload-images.jianshu.io/upload_images/1001659-7535c9e3fe16240d?imageMogr2/auto-orient/strip|imageView2/2/w/600/format/webp)

快乐学习

### 7.2. 参考式

**语法说明：**
 在文档要插入图片的地方写![图片Alt][标记]

在文档的最后写上[标记]:图片地址 "Title"

**代码：**



```ruby
快乐学习：
![快乐学习][study]

[study]:http://upload-images.jianshu.io/upload_images/1001659-7535c9e3fe16240d?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "快乐学习"
```

**显示效果：**
 快乐学习：

![img](https:////upload-images.jianshu.io/upload_images/1001659-7535c9e3fe16240d?imageMogr2/auto-orient/strip|imageView2/2/w/600/format/webp)

快乐学习


