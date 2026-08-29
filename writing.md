---
layout: default
title: 文章
permalink: /writing/
---

# 文章

<p style="margin:0 0 20px;"><a href="https://github.com/sheep213/sheep213.github.io/new/main/_posts" target="_blank" style="display:inline-block;background:#4f6df5;color:#ffffff;padding:8px 18px;border-radius:8px;text-decoration:none;">＋ 写新文章</a> <span style="color:#6b7280;font-size:0.85rem;">（仅你自己能操作）</span></p>

{% for post in site.posts %}
<article class="post-card">
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%Y年%m月%d日' }}</time>
  <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
</article>
{% endfor %}
