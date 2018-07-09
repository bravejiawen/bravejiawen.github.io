---
layout: post
title: 如何在Github中上传文件？
---


## 相关问题
怎么上传文件到github/如何利用git工具上传文件/怎么配置git工具/上传文件到github的git命令/GitHub的使用

## 背景
git最大的优势就是版本控制，再也不用最后版本123啦，github的账号需要翻墙才能注册，注册好之后，这里主要讲
- 怎么配置git工具
- 怎么下载github上的文件
- 怎么上传文件到github

## 详细介绍
### 1、git
不定期进行文件git是特别好的习惯啦。
#### windows系统
在Windows上使用Git，可以从Git官网直接[下载安装程序](https://git-scm.com/download/win)，然后按默认选项安装即可。

安装完成后，在开始菜单里找到“Git”->“Git Bash”，蹦出一个类似命令行窗口的东西，就说明Git安装成功！安装完成后，在命令行输入：github的用户名和邮箱

```
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"
```

### 2、本地与仓库进行关联
在github仓库里新建一个仓库，clone到本地。在文件夹右键可看到git bash here,即可打开当前文件夹位置的命令行窗口（ps:我目前打开终端用的是cmder），依次使用以下命令，即可看到本地下载了仓库内容。
```
$ git init
$ git clone 仓库地址 #仓库clone or download复制来的地址

```

![image.png](https://upload-images.jianshu.io/upload_images/3676517-b249402724be157c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

每次更改文件下的内容后，依次使用以下命令,文件就更新到GitHub仓库里啦。
```
$ git add .
$ git commit -m "本次修改备注"
$ git push
```

即使后面文件再更改，想要原始版本，在commits就能找到“本次修改备注”这个版本啦。
![image.png](https://upload-images.jianshu.io/upload_images/3676517-7b304a6aa9efcf77.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 注意事项
- 在与仓库关联后，进行push的位置最好是在关联的主目录下，例如本地python1文件夹与仓库"python1"关联，python1下有子文件夹ch1,在ch1文件夹下进行git再push,会出现一点点问题。
- 查看文件夹关联仓库 使用命令 git remote -v
- 仅为本人学习笔记。深入学习请参考[Git教程 - 廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)


## Changelog
- 20180709 初稿
