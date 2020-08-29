---
layout: post
title: Hyper-V 与 VirtualBox 冲突的解决方法
date: 2020-08-29 09:22:50 +0800
categories: Technology
tags:  Virtual Machine
img: 
---

蓝屏图就不贴了<img src="https://s1.ax1x.com/2020/07/28/aA6TOI.png" style="zoom:25%;" />

> P.S. Windows沙盒 与 MuMu模拟器 冲突的问题亦可用此方法解决，因为 Windows沙盒 基于 Hyper-V，MuMu 模拟器基于 VirtualBox



## 解决方法

> 关闭 Hyper-V

以管理员身份运行cmd，输入以下命令，重启

```cmd
bcdedit /set hypervisorlaunchtype off
```



## 备用

> 开启 Hyper-V

以管理员身份运行cmd，输入以下命令，重启

```cmd
bcdedit /set hypervisorlaunchtype auto
```

