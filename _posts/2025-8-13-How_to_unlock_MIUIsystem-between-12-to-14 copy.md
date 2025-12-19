---
title: 在MIUI12-14间的小米设备解锁bl & root
description: 狗操的 xiaomi fucked unlockbl ability in miui(0,11]
author: VeryrrDefine
date: 2025-8-13 21:00:00 +0800
categories: [Blog]
tags: [xiaomi, android, linux, bootloader, root]

math: true
mermaid: true
---

# 在 MIUI12-14 间的小米设备解锁 bl

此方法不适用于：

1. 不能更新到 miui12 以上版本的设备
2. 升级过 Hyper OS 的设备

## 开始

首先，确认以下系统版本是不是 miui12-14 的。

找到开发者设置，开启 oem 解锁开关。

找到设备解锁状态，点击“绑定账号与设备”按钮，绑定设备。

## 下载解锁工具

去此处下载：https://www.miui.com/unlock/index.html

## 解锁

首先打开解锁工具，登录设备，然后用 adb 连接手机

输入如下命令

```bash
adb reboot bootloader
```

进入到 fastboot 模式后，重新连接手机，安装驱动

点击解锁，两次继续需要等大概 10 几秒，就解锁成功了，然后会重置手机的数据

# Root

对于一般小米手机，都有版本对应的线刷包可以获取，小米的 rom 刷机包一般在这个网站： [https://xiaomirom.com/](https://xiaomirom.com/)

在对应的线刷包找到 boot.img 文件，保存。

## 下载 magisk

去作者的 repo 正式版列表下载，相比于去神秘地方下载，github 更安全。[https://github.com/topjohnwu/Magisk/releases/tag/v29.0](https://github.com/topjohnwu/Magisk/releases/tag/v29.0)

在手机上安装 Magisk，直接把 apk 文件安装到手机上。

打开 magisk 界面，点击上面的安装。

然后不勾选 recovery， 然后关闭强制加密，下一步，选择 boot.img 然后点击修补文件，在`/storage/emulated/0/`下有类似于 magisk_patched-xxx.img 的文件，传到电脑上。

## 刷入 boot 镜像

关闭手机，按住音量下键和电源键（或者输入`adb reboot bootloader`），进入 bootloader 模式（一般会写 fastboot）
然后输入`fastboot flash boot.img magisk_patched-....img`

刷入过程中不要拔出数据线

刷入完成后，输入`fastboot reboot`重启手机

## 确认是否 root

打开 magisk 界面，版本号应该不是无法获取了。
然后尝试打开一些需要 root 的软件，一般可以正常获取就是正常 root 了。你也可以尝试打开手机管家，可能会发现“系统被 ROOT”字样。
