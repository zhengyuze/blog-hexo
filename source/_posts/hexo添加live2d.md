---
title: hexo中加入live2d 看板娘
date: 2019-01-24 10:22
tags: [hexo,live2d]
categories: hexo
---

## 安装

在 Hexo 项目的根目录运行命令：
`npm install --save hexo-helper-live2d`
---

## 配置
在 Hexo 的 _config.yml 文件中添加配置。
```
live2d:
  enable: true
  pluginModelPath: assets/
  model:
    use: live2d-widget-model-epsilon2_1  #模板目录，在node_modules里
  display:
    position: right
    width: 150
    height: 300
  mobile:
    show: false  #是否在手机进行显示
```

## 下载模型
下载模型，模型名称如下，一些模型的预览可以访问[这里](https://huaji8.top/post/live2d-plugin-2.0/)
`npm install live2d-widget-model-hibiki`

## 配置模型
下载完之后，在Hexo根目录中新建文件夹live2d_models，然后在node_modules文件夹中找到刚刚下载的live2d模型，将其复制到live2d_models中，然后编辑配置文件中的model.use项，将其修改为live2d_models文件夹中的模型文件夹名称。
然后重新发布博客即可。
![](http://pmwkijiad.bkt.clouddn.com/1550125157913.jpg)



## 部署
`hexo clean && hexo g`
---

[参考1:hexo 添加live2d看板动画](https://www.jianshu.com/p/3a6342e16e57)
[参考2:掘金-在Hexo博客上添加可爱的Live 2D模型](https://juejin.im/post/5c35b01d6fb9a049ef26c488)
