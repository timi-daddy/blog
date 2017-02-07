# 首先说一下 HTML 表单是什么，为什么需要使用它。

form表单用于用户在页面中输入一些信息（通过<input>标签等），浏览器将该信息打包传送给服务器，由服务器的后端程序进行下一步处理：如返回给用户一些信息或者更新服务器数据库的内容等。

## 常用的input标签：
```
<input name="" type="text"> // 小段文字框
<input name="" type="checkbox" value=""> // 复选框
<input name="" type="email">  // Email输入框
<input name="" type="file"> // 选择本地文件控件
<input name="" type="hidden"> // 隐藏框，当表当被提交时也会提交内容，用户不可见
<input name="" type="image" src="" alt="" height="" width=""> // 带图片的提交按钮
<input name="" type="password"> // 密码输入框
<input name="" type="radio" value=""> // 单选框
<input type="reset"> // 表单重置按钮
<input type="submit"> // 表单提交按钮
<textarea name="" rows="" cols=""></textarea> // 大段文字框
```

* 比如我们想做一个注册页面，用户需要填写自己的用户名、密码、个人信息等，最后点提交。这就是一个form表单。

* 还有我们想做一个用户调查表，收集用户对产品的反馈，也需要用到表单。

* 总之表单的用处很多，基本上需要收集用户信息的地方都能用得上表单。

## 表单使用起来也很简单。

* 首先，整个表单必须被包裹在一个<form></form>标签里

* 然后必须在表单最下面有一个提交按钮<input type="submit">或<button></button>

* 然后根据你表单的目的加入各种<input>输入框、控件、按钮等，每一个<input>都需要一个name属性，有一个value属性（如果是直接输入内容的输入框，如<input type="text">就可以不用加value属性）。

* 这样做是为了对每个<input>形成一个key:value对，这样整个表单信息形成一个object数据类型，传给后台服务器上的程序进行处理。如果没有name和value，那么表单信息相应的input内容无法传给服务器，等于你白填了这个input

* 最后，对每个<input>最好都加上一个<label>标签，这样做有三个好处：

  1. 用户可以通过<label>里的内容知道这个<input>是干什么的

  2. 用户可以点击<label>里的文字内容直接focus该<input>

  3. 对于使用屏幕阅读器的视力障碍人士，可以方便的知道每个<input>是做什么的