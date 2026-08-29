---
layout: default
title: 首页
---

# 你好，我是{{ site.author }} 👋

这里是我的个人主页。我在这里写一些想法，也分享一些文件。

## 最近的文章

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: '%Y-%m-%d' }}
{% endfor %}

[查看全部文章 →](/writing/)
