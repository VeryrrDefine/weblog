---
title: 解密data分区
description: 如何解密data分区
author: VeryrrDefine
date: 2025-8-13 21:00:00 +0800
categories: [Blog]
tags: [xiaomi, android, linux, bootloader]
pin: true
math: true
mermaid: true
---

# 如何永久解密data分区
建议刷机前做好备份字库操作，防止出事故。

## 下载DRT工具
DRT工具在页面[https://jamcz.com/tutorial/wanji/](https://jamcz.com/tutorial/wanji/)然后找到“刷机(救砖)工具”，里面有个DRT选项。

DRT全称`DNA-rom-tools`

下载DRT，打开，
进入设置（输入`77`），
输入`4`（<4>  合成EXT4[0:自动计算/1:原大小]：0），输入`1`
输入`00`
创建一个工程

## 移除加密

分解vendor.img文件（要放img文件）

进入到 `vendor/etc`文件夹

找到fstab.*（file system tab）文件

修改`/dev/block/bootdevice/by-name/userdata`一栏

将`forceencrypt=footer`移除

## 打包并刷回

打包(按序输入`2`,`0`,`1`)

进入fastboot模式（可看解锁bl文章）

先禁用AVB2.0:`fastboot --disable-verity --disable-verification flash vbmeta 原本的vbmeta.img文件` （这一步很重要，否则后面会卡米无限重启）
然后刷入vendor输入`fastboot flash vendor vendor.img`

## 后面的准备工作

接下来最好是：

清除data数据（`fastboot erase userdata`）

进入twrp（`fastboot boot twrp.img`）

## twrp

设置语言， 保持只读，格式化Data分区，然后重启选项进入bootloader

再一次进入twrp（命令同上），确认data分区被格式化，然后重启至原厂recovery，清除数据，重启手机，立即重启

一般情况下就会进入恢复出厂设置界面

然后恢复magisk，安装MT管理器

## 测试加密是否存在

重启，进入fastboot，重新运行twrp，查看挂载情况是否有解密data分区选项，没有则说明已经解密

## Trivia

事实上，我在解除data分区的过程中经历了以下过程：
* 重启后输入未知的密码解密手机
* 手机刚过第一屏就重启
* 显示miui图标后卡图标

每个人在玩只因的过程中多多少少遇到过这些问题，所以备份字库格外重要。