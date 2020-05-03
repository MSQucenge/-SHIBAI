---
title: 新版Kali Linux的小配置（持续更新）
date: 2020-05-02 23:24:49
tags:
    - 渗透
categories:
    - 渗透
---

# 新版 Kali Linux 的小配置（持续更新）

## 菜鸡又开始了他的写作生涯，hhh，大家不要介意我身为菜鸡就嫌弃我写的东西啊，虽然没用，但是万一帮到你了呢？话不多说，开始整活：新版 Kali Linux 的使用须知，使用手册。此版本为 2019-4 版本 下载地址：

[官网](https://www.kali.org/downloads/)

[百度云：此版为 kali linux64 版本 提取码：pfw8](https://pan.baidu.com/s/1K-JK7K8zhuA-lrhiYllZ3w)

## 安装过程

本文安装过程使用的是虚拟机 VMware Workstation 15 Pro

1. 打开虚拟机新建虚拟机点击下一步![](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi9pbWFnZS0xMi5wbmc?x-oss-process=image/format,png)

2. 找到刚才下载的镜像文件 kali-linux-2019.4-amd64.iso 再次点击下一步 ![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi9pbWFnZS0xMy5wbmc?x-oss-process=image/format,png)

3. ![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9pbWcyMDE4LmNuYmxvZ3MuY29tL2Jsb2cvMTEyNDM1Ny8yMDE5MDcvMTEyNDM1Ny0yMDE5MDcxNDE3MTcyMzAyNy0zMTM1NjMyNTMuanBn?x-oss-process=image/format,png)

4. **注意**选择合适位置，这里需要存放几十 G 的虚拟磁盘文件

![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi8xMjMucG5n?x-oss-process=image/format,png)

![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi8xNTYwNzAwNjA4MS5wbmc?x-oss-process=image/format,png)

5. 设置虚拟磁盘的大小，一般不能低于默认值，下面一般选择单个文件，因为方便，新建完成，硬件可以之后自定义：

![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi9pbWFnZS0xNS5wbmc?x-oss-process=image/format,png)

![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi8xNTYwNzAwODEwMV8lRTUlODklQUYlRTYlOUMlQUMucG5n?x-oss-process=image/format,png)

**注**：觉得默认配置不合适可以自定义调整，例如修改内存大小，增加磁盘

**注**：设置网络适配器模式，可以桥接物理网络（例如电脑连接 wifi，虚拟机就和电脑连接同一个 wifi），或者 NAT 模式（类似于电脑成为一个路由器，虚拟机连接电脑的热点），如果不想联网，只用于物理机和虚拟机之间的交流，可以选择主机模式

6. 点击启动虚拟机

![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi8yMDE4MDQxNTE1MjMzNzI2MF8lRTUlODklQUYlRTYlOUMlQUMtMTAyNHg3MTYuanBn?x-oss-process=image/format,png)

7. 选中**Graphical install**

![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly93d3cubXhsLmluay93cC1jb250ZW50L3VwbG9hZHMvMjAxOS8wNi8xNTYwNzAxMDY0MS0xMDI0eDU1OS5wbmc?x-oss-process=image/format,png)

8. **注**：因为是新版本，对于我这类的菜鸡有点不友好，因为他的中文版本呈现出了乱码，因此我们选择英文版之后汉化（此处直接一路默认的过来哦就行，就不放图片咯，绝对不是因为我懒，大家都懂）
9. 期间需要漫长的等待
10. 基本大功告成了，基本上长这样![img](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9pbWFnZS4zMDAxLm5ldC9pbWFnZXMvMjAxOTExMzAvMTU3NTEwMDYwOF81ZGUyMjBjMDBiN2RmLmpwZyFzbWFsbA?x-oss-process=image/format,png)

## 开始调试工作

### 首先介绍这个版本的亮点：

此版本和之前相比变动很大，系统界面、主题、壁纸都灿然一新：最明显的变化是从`Gnome`迁移到`Xfce`作为默认桌面，`Kali Undercover`模式（能够伪装成`win10`）

### 更新功能

- 一个新的默认桌面环境，`Xfce`
- 新的 GTK3 主题(用于 Gnome 和 Xfce)
- `Kali Undercover`模式介绍
- `Kali`文档有了一个新家，现在支持`Git`
- 公共包装-把你的工具放进`Kali`
- 安装在`Android上`的 NetHunter Kex – Full Kali 桌面
- 安装过程中的`BTRFS`
- 添加`PowerShell`
- 内核升级到`5.3.9`版本
- ...以及常规的错误修复和更新。

#### 体验间谍模式（win 10 模式）

如果你在某些环境中想用 Kali 做点什么，却又不想被人轻易发现，，（大家都懂），那就顺手打开间谍模式吧，hhh

神秘代码：Kali Undercover

自己体验吧，我就不放图了

再次运行脚本就可以重新切换回之前的主题。此外，在桌面也可以直接搜索到这条命令

### 换国内源

换上国内源就可以体验到比较快的下载速度了（相对来说）

进入 /etc/apt/ sources.list

把下列代码复制进 sources 文件

```脚本
#

#aliyun 阿里云
deb http://mirrors.aliyun.com/kali kali-rolling main non-free contrib
deb-src http://mirrors.aliyun.com/kali kali-rolling main non-free contrib

# ustc 中科大
deb http://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
deb-src http://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
#deb http://mirrors.ustc.edu.cn/kali-security kali-current/updates main contrib non-free
#deb-src http://mirrors.ustc.edu.cn/kali-security kali-current/updates main contrib non-free

# kali 官方源
deb http://http.kali.org/kali kali-rolling main non-free contrib
deb-src http://http.kali.org/kali kali-rolling main non-free contrib

# 默认的，可以注释掉不用管
#deb http://security.kali.org/kali-security kali-rolling/updates main contrib non-free
#deb-src http://security.kali.org/kali-security kali-rolling/updates main contrib non-free
```

我采用的是阿里云和中科大的国内源

### 开始汉化

1. 更新源和软件 apt-get update && apt-get upgrade && apt-get clean

2. 选语言 dpkg-reconfigure locales 进入图形界面，选中 en_US.UTF-8 UTF-8 和 zh_CN.UTF-8 UTF-8（空格是选择，tab 是切换，\*是选中）并将 zh_US.UTF-8 选为默认。
3. 安装中文字体 apt-get install xfonts-intl-chinese apt-get install ttf-wqy-microhei **安装中文字体非常重要**
4. 重启 reboot （重启还是英文，就继续重启，基本一到两次后就可以了）

### 安装强大的 PowerShell

神秘代码：apt update && apt -y install powershell

### 安装汉语拼音

**神秘代码**：apt-get install fcitx fcitx-googlepinyin

1.  输入神秘代码
2.  重启
3.  打开 fcitx 设置
4.  把谷歌拼音放到最上面

## 好了第一次更新，已经做完了，基本上是 Kali Linux 的基本微操，如果有我想到的我会持续更新，kali 已经下载了，说明搞事就快要开始咯，hhh，这次就不水文章了，如果大家有什么好玩的骚操作可以私聊我哦，欢迎大神来骚扰
