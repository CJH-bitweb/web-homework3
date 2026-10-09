# 实验3 CSS布局实战——导航菜单

## 一、作业内容
在不修改 HTML 结构的前提下，仅用 CSS 将两个给定文件改造成水平导航菜单：一级菜单用表格布局，二级菜单用 ul/li 结构并含下拉子菜单。

## 二、使用到的标签与知识点
标签：`<table>`、`<tr>`、`<td>`、`<ul>`、`<li>`、`<a>`。
CSS：类选择器、后代选择器、`:hover` 伪类、盒模型、`display: flex/block/none`、`position: relative/absolute`、`z-index`。

## 三、遇到的困难及解决方法
1. 二级菜单默认显示占位 → 用 `display: none` 隐藏，`li:hover > ul` 显示。
2. 下拉位置乱跑 → 父 `li` 加 `relative`，子 `ul` 加 `absolute` 并 `top: 100%`。
3. 鼠标移到二级菜单就消失 → 让子菜单紧贴父项，不留间隙。

## 四、验证
Live Server 打开两个页面，悬停变色、二级菜单下拉显示正常。