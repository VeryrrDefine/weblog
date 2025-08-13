---
title: 在MIUI12-14间的小米设备解锁bl & root
description: 狗操的 xiaomi fucked unlockbl ability in miui(0,11]
author: VeryrrDefine
date: 2025-8-13 21:00:00 +0800
categories: [Blog]
tags: [xiaomi, android, linux, bootloader, root]
pin: true
math: true
mermaid: true
---

# 在MIUI12-14间的小米设备解锁bl

此方法不适用于：
1. 不能更新到miui12以上版本的设备
2. 升级过Hyper OS的设备

## 开始
首先，确认以下系统版本是不是miui12-14的。

找到开发者设置，开启oem解锁开关。

找到设备解锁状态，点击“绑定账号与设备”按钮，绑定设备。

## 下载解锁工具
去此处下载：https://www.miui.com/unlock/index.html

## 解锁

首先打开解锁工具，登录设备，然后用adb连接手机

输入如下命令
```bash
adb reboot bootloader
```
进入到fastboot模式后，重新连接手机，安装驱动

点击解锁，两次继续需要等大概10几秒，就解锁成功了，然后会重置手机的数据

# Root

对于一般小米手机，都有版本对应的线刷包可以获取，小米的rom刷机包一般在这个网站： [https://xiaomirom.com/](https://xiaomirom.com/)

在对应的线刷包找到boot.img文件，保存。

## 下载magisk

去作者的repo正式版列表下载，相比于去神秘地方下载，github更安全。[https://github.com/topjohnwu/Magisk/releases/tag/v29.0](https://github.com/topjohnwu/Magisk/releases/tag/v29.0)

在手机上安装Magisk，直接把apk文件安装到手机上。

打开magisk界面，点击上面的安装。

然后不勾选recovery， 然后关闭强制加密，下一步，选择 boot.img然后点击修补文件，在`/storage/emulated/0/`下有类似于magisk_patched-xxx.img的文件，传到电脑上。

## 刷入boot镜像

关闭手机，按住音量下键和电源键（或者输入`adb reboot bootloader`），进入bootloader模式（一般会写fastboot）
然后输入`fastboot flash boot.img magisk_patched-....img`

刷入过程中不要拔出数据线

刷入完成后，输入`fastboot reboot`重启手机

## 确认是否root

打开magisk界面，版本号应该不是无法获取了。
然后尝试打开一些需要root的软件，一般可以正常获取就是正常root了。你也可以尝试打开手机管家，可能会发现“系统被ROOT”字样。