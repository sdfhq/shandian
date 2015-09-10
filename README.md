# shandian

闪电孵化器新官网 DEMO - Powered by Jekyll 

You can preview here: http://sd.ycz.im  

## 维护方式

由于站点，采用纯静态方式。所以没有相应的后台管理面板。需要对 Repo 直接操作。

这里以网站有几种维护需求为例说明：

* 更新/创建「Startup」项目
* 更新/创建「Post」文章
* 更新/创建「Page」页面

---

## 目录结构

```
_includes: 
_layouts:
_posts: 放文章文件
_sass:
_startup: 放 startup 项目文件
about: About 相关页面文件
  - cooperators.md: 合作伙伴
  - members.md: 团队成员
  - joinus.md: 加入我们
  - nibachuangke.md: 泥巴创客
  - service-organization.md: 服务机构
assets
blog
service
  - activity.md: 活动
  - apply.md: 申请孵化
  - course.md: 创业课程
  - rules.md: 入驻规则

  - activity: 活动子项目
    - startup-training-2014.md
  - course: 课程子项目
    - programming-practice-2014.md
    - programming-practice-2014.md
    - learning-materials.md
sync
_config.yml
about.md: 关于页面
blog.md: 博客页面
index.html: 首页
service.md: 服务页面
startup-archived.md: 归档项目
startup.md: 孵化项目
```


## tartup 类型

```
---
layout: startup
title:  "项目名称"
date:   2013-11-01 14:05:17
cover:	项目图片名.jpg/png
desc:	这里是项目简要描述
addr:	地点
invest:	融资说明
team:	
  - name: 成员A
    position: "职称"
    desc: 描述
  - name: 成员B
    avatar: 
    position: "职称"
    desc: 描述
progress:
  - date: 2012年
    desc: 描述
  - date: 2013年6月
    desc: 描述
contact: lalala@gmail.com
archive: true (true 为归档，不写为非归档)
---

这里写正文部分

```

以上 meta 信息中，`invest`、`team`、`progress`、`contact`、`archive` 都是非必填项。

如何新建一个 Startup ：

> 1. 在 `_startup` 文件夹下创建一个 xxx.markdown 文件
>
> 2. 按上述格式要求填写
>
> 3. 预览，保存


## post 类型

```
---
layout: post
title: 闪电孵化器官方网站上线
author: admin
permalink: /2013/11/official-website-release/
categories: [新闻]
---

这里写正文

```

如何新建一篇文章：

> 1. 在 `_posts` 文件夹下新建一个 xxx.md 文件
>
> 2. 按照上述要求填写
> 
> 3. 预览，保存


## page 类型

page 类型，稍微复杂。当前站点拥有的 page 层级如下，可以修改需要的 markdown 文件内容。

```
service.md
about.md。
startup.md
blog.md

service
  - activity.md
  - apply.md
  - course.md
  - rules.md

  - activity
    - startup-training-2014.md
  - course
    - programming-practice-2014.md
    - programming-practice-2014.md
    - learning-materials.md

about
  - cooperators.md
  - members.md
  - joinus.md
  - nibachuangke.md
  - service-organization.md
```


如何创建新的 Page：

> 1. 选择合适的文件夹，创建 markdown 文件
>
> 2. 给 markdown 文件里，指定合适的 permalink 链接
> 
> 3. 修改 layout/service.html 或者 layout/about.html，给刚创建的页面添加链接指向。





