---
layout: default
title: 文件
permalink: /files/
---

# 文件

<p style="margin:0 0 20px;"><a href="https://github.com/sheep213/sheep213.github.io/upload/main/files" target="_blank" style="display:inline-block;background:#4f6df5;color:#ffffff;padding:8px 18px;border-radius:8px;text-decoration:none;">⬆ 上传文件</a> <span style="color:#6b7280;font-size:0.85rem;">（仅你自己能操作）</span></p>

这里是可以下载的文件。把文件放进 `files` 文件夹，就会自动出现在下面的列表里。

<ul class="file-list">
{% assign files = site.static_files | where_exp: "f", "f.path contains '/files/'" %}
{% for f in files %}
  <li>
    <a href="{{ f.path | relative_url }}">{{ f.name }}</a>
    <span class="file-meta">{{ f.extname | remove_first: '.' | upcase }} · {{ f.modified_time | date: '%Y-%m-%d' }}</span>
  </li>
{% endfor %}
</ul>

如果上面是空的，说明还没有上传文件。
