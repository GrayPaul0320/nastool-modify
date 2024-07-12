# 让群晖NASTOOL套件支持MT的新api

## 原理	

修改底层代码，请做好备份，本教程不为任何结果负责

## 准备工作

1、按照http://www.ptyqm.com/27850.html，以便让自己可以使用winscp，root账号登录群晖NAS，以方便修改底层文件

2、有一些代码基础，最好是python代码基础

3、套件版本3.4.0

## 找到nastool的底层文件

1、理论上应该是/volume*(安装套件的存储空间名)/@appstore/NASTool/nas-tools/app

2、按照joneechua大佬更新的代码，修改自己nas中的代码。https://github.com/joneechua/nas-tools/commit/ee7caf559c243ce6f7e0ca35ff9e3c2153f6044b

![image-20240712124629019](https://typora-1255648391.cos.ap-beijing.myqcloud.com/img/image-20240712124629019.png)

主要涉及上面这四个文件

可以自己对照着修改，也可以使用我修改好的代码