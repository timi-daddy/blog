# 有哪些常见的 meta 标签

## 先说一下 <meta> 元素是什么。

* 凡是在 <head> 元素中，不能用这几个元素 (<base>, <link>, <script>, <style>, <title>) 来表示的元数据，都要用 <meta> 元素来表示。

## 再说一些常见的 <meta> 元素类型。

1. <meta charset="utf-8"> // 指定字符集
2. <meta name="keywords" content=""> // 向搜索引擎说明你的网页的关键词
3. <meta name="description" content=""> // 告诉搜索引擎你的站点的主要内容
4. <meta name="author" content="你的姓名"> // 告诉搜索引擎你的站点的制作的作者
5. <meta name="viewport" content="width=device-width, initial-scale=1.0"> // 响应式页面
6. <meta http-equiv="refresh" content="3;url=https://www.mozilla.org"> //定时让网页在3秒内跳转到mozilla首页
7. <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"> // 如果安装了GCF (Google Chrome Frame)，则使用GCF来渲染页面 ("chrome=1"), 如果没有安装GCF，则使用最高版本的IE内核进行渲染 ("IE=edge")。