---
title: Vim简单运用
date: 2020-05-02 23:26:39
tags:
    - 笔记
categories:
    - 笔记
---

# Vim 笔记

## Vim 特点：

- 功能强大、高度可定制
- vim=vi+improved

## Vim 功能：

- 多级撤销
- 语法加亮和自动补全
- 支持多种插件
- 通过网络协议(HTTP/SSH)编辑文件
- 多文件编辑
- 可同时编辑压缩格式文件(gzip、zip 等)

### Vim 的四种模式

- 普通模式 ：打开默认模式；移查删改
- 可视化模式 ：对一整快区域进行操作
- 插入模式 ： 添加文本
- 命令模式 ：

## Vimrc 简介

- rc=run command（运行命令）
- 系统级 Vimrc 和用户级 Vimrc
- 每一行作为一个命令执行

### Vimrc 使用

- ：version
- :e~/.vimrc
- “注释
- :vimrc-sample

### Vim 中移动跳转与缩进

#### 光标的移动

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204203900817.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

#### 单词及字符的移动

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204203938431.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)![在这里插入图片描述](https://img-blog.csdnimg.cn/2020020420403290.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

### 缩进

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020020420411347.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

### Vim 的删除复制与粘贴

#### Win 与 Vim 差异

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204204134196.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

#### 基本操作

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204204158503.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70) ####　比较详细的基本操作

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204204220795.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

#### 调换字符

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020020420423044.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

#### 行剪切粘贴

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204204258889.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

#### Vim 组合删除

公式：([count]operation([count]{motion})

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204204402458.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/2020020420444379.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

## 基础部分

### Vim 寄存器

vim 中保存临时数据的地方

#### 寄存器种类

1. 无名寄存器
2. 数字寄存器
3. 有名寄存器
4. 黑洞寄存器

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204204503416.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200204204523683.png)

### Vim 增删改查

详见上文，此处为原来大纲，暂未更改

### Vim 组合规律

Vim 一系列组合键操作

同上

## Vim 高级功能

### 缓冲区和多文件的编辑

#### 缓冲区

Buffer 是内存中的一块缓冲区域，用于临时存放 Vim 打开过的文件

#### 缓冲区列表

-　 files -　 buffers -　 ls

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-TV1TOz6T-1580990092997)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_020.png)]](https://img-blog.csdnimg.cn/20200206195515545.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200206195544357.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)![在这里插入图片描述](https://img-blog.csdnimg.cn/20200206195600272.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

### 多窗口与标签分组

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-oFtJjSmJ-1580990092999)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_023.png)]](https://img-blog.csdnimg.cn/20200206195714332.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

#### 标签

容纳一系列窗口的容器

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-qoWTqneI-1580990093001)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_024.png)]](https://img-blog.csdnimg.cn/20200206195725705.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-kGFGmKdA-1580990093002)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_025.png)]](https://img-blog.csdnimg.cn/20200206195755880.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

### 文本对象和宏

#### 文本对象

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-DDJqrIcT-1580990093002)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_026.png)]](https://img-blog.csdnimg.cn/20200206195840274.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-AA9SvZzq-1580990093003)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_027.png)]](https://img-blog.csdnimg.cn/20200206195900897.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-yOB0OUpt-1580990093004)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_029.png)]](https://img-blog.csdnimg.cn/202002061959176.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200206195939263.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200206195959863.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

#### 宏

可以理解为自定义的操作，例如鼠标宏，或者王者荣耀中的一键换装

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020020620003198.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)
![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-9QfZgGEl-1580990093006)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_032.png)]](https://img-blog.csdnimg.cn/20200206200045791.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200206200109784.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1OTg4NQ==,size_16,color_FFFFFF,t_70)

### Visaual 模式（可视化模式）

可对文本块整体的进行操作

#### 三种子模式

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200206200125566.png)

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-FnmqZzXb-1580990093006)(Vim%E7%AC%94%E8%AE%B0.assets/%E9%80%89%E5%8C%BA_035.png)]](https://img-blog.csdnimg.cn/20200206200127282.png)

可视化模式有很多扫操作，这里就不意义举例了，大家如果有神么好的操作可以可以留言哦

