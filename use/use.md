### 效果：

![image.png](https://upload-images.jianshu.io/upload_images/6025530-c1b10fbbdb0fbda3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 步骤：

1、Fork **[SimpleTheme](https://github.com/lcfu1/SimpleTheme)** 到你的github上。
2、到Settings中点击Choose a theme随便选择一个theme。

![image.png](https://upload-images.jianshu.io/upload_images/6025530-d3cf51e17b786b72.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

3、打开_config.yml进行配置，如下。

```
#title必须设置和github上该repository的name一致，如果该repository name为"用户名.github.io"，则不需要填。
title: SimpleTheme

#author设置为github用户名
author: lcfu1

description: SimpleTheme

#把下面这个theme注释掉
#theme: jekyll-theme-cayman
```

4、README.md就是该Github Pages的主页，打开README.md进行编辑（可根据自己的需要进行修改），不过我希望能够统一按照下面例子进行修改：

```
# {{ site.title }}

> Description：{{ site.description }}
>
> author：{{ site.author }}
>
> <a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/subscription" data-show-count="true" aria-label="Watch {{ site.author }}/{{ site.title }} on GitHub">Watch</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}" data-show-count="true" aria-label="Star {{ site.author }}/{{ site.title }} on GitHub">Star</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/fork" data-show-count="true" aria-label="Fork {{ site.author }}/{{ site.title }} on GitHub">Fork</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/issues" data-show-count="true" aria-label="Issue {{ site.author }}/{{ site.title }} on GitHub">Issue</a>
<a class="github-button" href="https://github.com/{{ site.author }}" data-show-count="true" aria-label="Follow @{{ site.author }} on GitHub">Follow @{{ site.author }}</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/archive/master.zip" aria-label="Download {{ site.author }}/{{ site.title }} on GitHub">Download</a>

## Theme

- SimpleTheme

	- [使用说明](use/use.md)
```

5、end