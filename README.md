精通：nth-child
==============

## :nth-child

:nth-child(8) 选中第八个子元素

```css

li:nth-child(8) span {
    background-color: #298EB2;
    box-shadow: -3px -3px 10px rgba(0, 0, 0, 0.4), inset 0 0 10px black;
}

```

使用**:nth-child(8)**可以让你选中父元素下唯一的第八个子元素

## :nth-child 范围用法

### 正方向范围

:nth-child(n+6)选中从第六个开始的子元素

```css

li:nth-child(n+6) span {
    background-color: #298EB2;
    box-shadow: inset -3px -3px 10px rgba(0, 0, 0, 0.4), 0 0 10px black;
}

```

使用**:nth-child(n+6)**，就相当于选中了第六个**:nth-child(6)**和其后面的所有子元素

### 负方向范围

**:nth-child(-n+9)**选中从第一个到第九个子元素

```css

li:nth-child(-n+9) span {
    background-color: #298EB2;
    box-shadow: inset -3px -3px 10px rgba(0, 0, 0, 0.4), 0 0 10px black;
}


```

### 前后限制范围

**nth-child(n+4):nth-child(-n+8)**选中第4-8个子元素

```css

li:nth-child(n+4):nth-child(-n+8) span {
    background-color: #298EB2;
    box-shadow: inset -3px -3px 10px rgba(0, 0, 0, 0.4), 0 0 10px black;
}


```

使用**nth-child(n+4):nth-child(-n+8)**我们可以选中某一范围内子元素

## 范围高级用法

**nth-child(n+2):nth-child(odd):nth-child(-n+9)**奇数位/偶数位子元素

```css

li:nth-child(n+2):nth-child(odd):nth-child(-n+9) span {
    background-color: #298EB2;
    box-shadow: inset -3px -3px 10px rgba(0, 0, 0, 0.4), 0 0 10px black;
}

```

使用**nth-child(n+2):nth-child(odd):nth-child(-n+9)**我们将会选中的子元素是从第2位到第9位，并且只包含奇数位。

## nth-child(3n+1):nth-child(even)间隔选择子元素

```css

li:nth-child(n+2):nth-child(odd):nth-child(-n+9) span {
    background-color: #298EB2;
    box-shadow: inset -3px -3px 10px rgba(0, 0, 0, 0.4), 0 0 10px black;
}


```

使用**nth-child(3n+1)**我们可以每个三个选中一个，也就是第1,4,7和10个子元素，但通过使用**nth-child(even)**我们可以过滤掉基数为子元素，也就是1和7，于是就剩下子元素只有4和10.

## :nth-of-type 的用法

明天再写吧，今天有点晚了。明天要在家一个示例页面才行。光说没啥说服力。

http://www.webhek.com/post/mastering-nth-child.html



