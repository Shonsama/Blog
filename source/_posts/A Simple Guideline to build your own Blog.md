---
title: A Simple Guideline to build your own Blog
date: 2020-11-16 17:22:47
tag: [Hexo, Blog]
categories: 计算机
index_img: /img/index/Hexo.png
---
Welcome to My Blog! This is my very first post. In this post, a simple guideline of using Hexo and fluid to build and beatify your own Blog will be provided. If you have any question, please check the [Hexo offical document](https://hexo.io/docs/) and [Fluid offical document](https://hexo.fluid-dev.com/docs) for more detailed information.

## The Environment
### Install Git
Download Git in the offical website: [Git - Downloading Package](https://git-scm.com/download/win).
### Install Node.js
Download Node.js in the offical website: [Download | Node.js](https://nodejs.org/en/download/).
## Init Hexo Project
### Install hexo-cli
``` bash
$ npm install -g hexo-cli 
```
### Init hexo project
``` bash
$ hexo init blog 
```
### Create a new post

``` bash
$ hexo new "Post Name"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server
Show the website in localhost.
``` bash
$ hexo s
```

More info: [Server](https://hexo.io/docs/server.html)
### Config deployment
Open the file `_config.yml` in folder `/themes` and modify the deploy part as follows:
``` bash
deploy:
    type: git
    repo: 'your repository URL'
    branch: master
```
### Save the configuration file
``` bash
$ npm install hexo-deployer-git --save
```
### Clean static files

``` bash
$ hexo clean
```


### Generate static files

``` bash
$ hexo g
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo d
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
## Using Theme Fluid
### Install Fluid
If your Hexo version >= 5.0.0, you can install Fluid via Npm:
``` bash
$ npm install --save hexo-theme-fluid
```
Then create `_config.fluid.yml` in the blog directory and copy the content of `_config.yml` in [Page](https://github.com/fluid-dev/hexo-theme-fluid/blob/master/_config.yml).
### Set theme

Edit `_config.yml` in the blog root directory as follows:
```
theme: fluid
```
### Create about page
The about page needs to be created manually:
``` bash
$ hexo new page about
```

Then edit `/source/about/index.md` and add `layout` attribute.
The modified example is as follows:
```
---
title: about
date: 2020-02-23 19:20:33
layout: about
---

About content
```
### More configuration
For more information, please visit the [Offical document](https://hexo.fluid-dev.com/docs/guide/#%E5%85%B3%E4%BA%8E%E6%8C%87%E5%8D%97).