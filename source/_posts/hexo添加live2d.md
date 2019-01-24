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

## 部署
`hexo clean && hexo g`
---

[参考:hexo 添加live2d看板动画](https://www.jianshu.com/p/3a6342e16e57)
