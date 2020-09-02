## 代码

对于程序员来说这个功能是必不可少的，插入程序代码的方式有两种，一种是利用缩进(Tab), 另一种是利用“`”符号（一般在ESC键下方）包裹代码。

**语法说明：**

1. 插入行内代码，即插入一个单词或者一句代码的情况，使用`code`这样的形式插入。
2. 插入多行代码，可以使用缩进或者``` code ```,具体看示例。

**注意： 缩进式插入前方必须有空行**

### 13.1. 行内式

**代码：**



```cpp
C语言里的函数 `scanf()` 怎么使用？
```

**显示效果：**

C语言里的函数 `scanf()` 怎么使用？

### 13.2. 缩进式多行代码

缩进 4 个空格或是 1 个制表符

一个代码区块会一直持续到没有缩进的那一行（或是文件结尾）。

**代码：**



```cpp
    #include <stdio.h>
    int main(void)
    {
        printf("Hello world\n");
    }
```

**显示效果：**



```cpp
#include <stdio.h>
int main(void)
{
    printf("Hello world\n");
}
```

### 13.3. 用六个`包裹多行代码

**代码：**

\```
 \#include <stdio.h>
 int main(void)
 {
 printf("Hello world\n");
 }
 \```

**显示效果：**



```cpp
#include <stdio.h>
int main(void)
{
    printf("Hello world\n");
}
```

### 13.4. 代码高亮

代码高亮示例:



```javascript
/**
* nth element in the fibonacci series.
* @param n >= 0
* @return the nth element, >= 0.
*/
function fib(n) {
  var a = 1, b = 1;
  var tmp;
  while (--n >= 0) {
    tmp = a;
    a += b;
    b = tmp;
  }
  return a;
}
 
document.write(fib(10));
```



```python
class Employee:
   empCount = 0
 
   def __init__(self, name, salary):
        self.name = name
        self.salary = salary
        Employee.empCount += 1
```

### 13.5. HTML 原始码 （*注：简书Markdown不支持HTML原始码*）

在代码区块里面， & 、 < 和 > 会自动转成 HTML 实体，这样的方式让你非常容易使用 Markdown 插入范例用的 HTML 原始码，只需要复制贴上，剩下的 Markdown 都会帮你处理，例如：

**代码：**

第一个例子：



```csharp
<div class="footer">
   © 2004 Foo Corporation
</div>
```

第二个例子：



```xml
<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>
```

**显示效果：**

第一个例子：

![img](https:////upload-images.jianshu.io/upload_images/1001659-0270afa6180253e3.png?imageMogr2/auto-orient/strip|imageView2/2/w/207/format/webp)

HTML源码效果

第二个例子：

![img](https:////upload-images.jianshu.io/upload_images/1001659-fc5bf3320d05a673.png?imageMogr2/auto-orient/strip|imageView2/2/w/329/format/webp)

HTML表格

