---
layout: post
title: 如何在Github中/md文件中上传图片？
---

## 背景
如何在github仓库的`` .md``文件里上传图片？据说七牛云作为图床最方便，但是配置过程比较折腾，介绍目前知道的几种方法。
- 新浪微博相册做图床
- github建照片文件夹
- 简书

## 详细介绍

#### 1、简书
我目前用的是简书，就是图方便，打开简书的写文章界面，复制图片到文件里，自动上传得到一个地址
![image.png](https://upload-images.jianshu.io/upload_images/3676517-0ed24efb27aeb698.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

```
(![image.png](https://upload-images.jianshu.io/upload_images/3676517-7cbc81db36b891bc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#复制这个地址到.md文件里就可以了，保存草稿，不用发表。
```

#### 2、github建照片文件夹
#github新手不会上传文件请移步 [github怎么上传文件？]()
- 上传图片到github文件夹，打开图片，右键``复制图片地址``,按markdown格式![](图片地址)，即可插入到md文件里。
- 这里可能需要注意，如果直接复制地址栏里的地址不一定可以
- 由于个人写报告期间经常用到截图，上传到文件夹里并没有简书那么方便，如果有好的办法，欢迎交流。447969255@qq.com


#### 3、新浪微博

图片传到微博相册，右键图片，在新标签页打开，复制照片网址，``.jpg``或者别的图片格式结尾的哦，然后在md文件里编辑如下，即得到下面的图片。但是私密的不一定能够看到，最好是一个单独拿来存图片的微博。

```
![此处可自己随意填写](http://wx2.sinaimg.cn/mw690/d7071319ly1fn4yfsgpp2j20vk0hs0v5.jpg)
```

![此处可自己随意填写.jpg](
http://wx2.sinaimg.cn/mw690/d7071319ly1fn4yfsgpp2j20vk0hs0v5.jpg)

## 新手参考
1、可适用于直接在github网页中编辑文件。
2、编辑markdown文件时做图床，因为图片没有地址是无法上传到markdown文件里的。
3、记得把文件后缀改为.md

## CHANGELOG
- 20180709 初稿
