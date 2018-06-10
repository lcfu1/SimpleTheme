# 使用说明

### 效果：

![SimpleTheme](https://raw.githubusercontent.com/lcfu1/Image/master/Use/SimpleTheme.PNG)

### 步骤：

1、Fork **[SimpleTheme](https://github.com/lcfu1/SimpleTheme)** 到你的github上。

2、到Settings中点击Choose a theme随便选择一个theme。

![SimpleTheme-Theme](https://raw.githubusercontent.com/lcfu1/Image/master/Use/SimpleTheme-Theme.png)

3、打开_config.yml进行配置，如下。

```
#title必须设置和github上该repository的name一致，如果是 用户.github.io，则可以不填。
title: SimpleTheme

#author设置为github用户名
author: lcfu1

#记得把下面这个theme注释掉
#theme: jekyll-theme-cayman

#这里的Application ID和REST API Key可以通过注册bmob，然后新建一个项目，从而获得该项目的Application ID和REST API Key，用于统计文章阅读次数。
#Application ID
id: d6f5df1e30903a0a49634f3ac9c96ecf

#REST API Key
key: 29bc5d837e8c6054da46fde3ddfce1c8

#这里的table填写的表名要跟bmob上新建的表名一样
table: SimpleTheme
```

4、README.md就是该Github Pages的主页，打开README.md进行编辑（可根据自己的需要进行修改）。