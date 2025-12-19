---
title: 解密data分区
description: 如何解密data分区
author: VeryrrDefine
date: 2025-8-13 21:00:00 +0800
categories: [Blog]
tags: [xiaomi, android, linux, bootloader]

math: true
mermaid: true
---

# 如何永久解密 data 分区

建议刷机前做好备份字库操作，防止出事故。

## 下载 DRT 工具

DRT 工具在页面[https://jamcz.com/tutorial/wanji/](https://jamcz.com/tutorial/wanji/)然后找到“刷机(救砖)工具”，里面有个 DRT 选项。

DRT 全称`DNA-rom-tools`

下载 DRT，打开，
进入设置（输入`77`），
输入`4`（<4> 合成 EXT4[0:自动计算/1:原大小]：0），输入`1`
输入`00`
创建一个工程

## 移除加密

分解 vendor.img 文件（要放 img 文件）

进入到 `vendor/etc`文件夹

找到 fstab.\*（file system tab）文件

修改`/dev/block/bootdevice/by-name/userdata`一栏

将`forceencrypt=footer`移除

## 打包并刷回

打包(按序输入`2`,`0`,`1`)

进入 fastboot 模式（可看解锁 bl 文章）

先禁用 AVB2.0:`fastboot --disable-verity --disable-verification flash vbmeta 原本的vbmeta.img文件` （这一步很重要，否则后面会卡米无限重启）
然后刷入 vendor 输入`fastboot flash vendor vendor.img`

## 后面的准备工作

接下来最好是：

清除 data 数据（`fastboot erase userdata`）

进入 twrp（`fastboot boot twrp.img`）

## twrp

设置语言， 保持只读，格式化 Data 分区，然后重启选项进入 bootloader

再一次进入 twrp（命令同上），确认 data 分区被格式化，然后重启至原厂 recovery，清除数据，重启手机，立即重启

一般情况下就会进入恢复出厂设置界面

然后恢复 magisk，安装 MT 管理器

## 测试加密是否存在

重启，进入 fastboot，重新运行 twrp，查看挂载情况是否有解密 data 分区选项，没有则说明已经解密

## Trivia

事实上，我在解除 data 分区的过程中经历了以下过程：

- 重启后输入未知的密码解密手机
- 手机刚过第一屏就重启
- 显示 miui 图标后卡图标

每个人在玩只因的过程中多多少少遇到过这些问题，所以备份字库格外重要。
