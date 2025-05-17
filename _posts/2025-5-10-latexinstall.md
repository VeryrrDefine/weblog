---
title: 在Termux上安装manim
description: installing manim
author: VeryrrDefine
date: 2025-5-10 16:48:00 +0800
categories: [python]
tags: [python, math, manim]
pin: true
math: true
mermaid: true
---
# 安装
## 安装latex
数学公式是manim所需要的，latex是用于渲染公式的。
### 安装texlive
安装texlive输入
```shell
apt i texlive-bin
```
其中的`texlive-bin`可以换成`texlive-installer`。

包安装完后，输入`termux-install-tl`, 按C
出现`start installation to hard disk`时按I(第8个英语字母)。

接下来耐心等待，可能需要花费一个小时以上。
 
安装完后，输入`termux-patch-texlive`, 修复部分脚本的`/tmp`。

### 重建软连接
如果输入`tex` 正常，而输入latex不行，需要重建软连接。
```shell
ln -s luatex dvilualatex
ln -s pdftex latex
ln -s luahbtex lualatex
ln -s pdftex pdflatex

```

## manim
```shell
pip install manim
```
