---
title: 在Termux上安装manim
description: installing manim
author: VeryrrDefine
date: 2025-5-10 16:48:00 +0800
categories: [python]
tags: [python, math, manim]

math: true
mermaid: true
---

# 安装

## 安装 latex

数学公式是 manim 所需要的，latex 是用于渲染公式的。

### 安装 texlive

安装 texlive 输入

```shell
apt i texlive-bin
```

其中的`texlive-bin`可以换成`texlive-installer`。

包安装完后，输入`termux-install-tl`, 按 C
出现`start installation to hard disk`时按 I(第 8 个英语字母)。

接下来耐心等待，可能需要花费一个小时以上。

安装完后，输入`termux-patch-texlive`, 修复部分脚本的`/tmp`。

### 重建软连接

如果输入`tex` 正常，而输入 latex 不行，需要重建软连接。

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
