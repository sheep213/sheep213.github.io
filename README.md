# 我的个人主页 · 使用说明

这是一个不需要你会写代码的个人主页，包含三个部分：

- 首页：自我介绍 + 最近的文章
- 文章：像写日记一样写点东西
- 文件：上传和下载文件

## 一、怎么把它放到网上（免费，推荐 GitHub Pages）

1. 注册一个 GitHub 账号：打开 https://github.com ，点右上角 Sign up，用邮箱注册。
2. 登录后，点右上角「+」→「New repository」（新建仓库）。
3. 仓库名字填：`你的用户名.github.io`
   （把「你的用户名」换成你的 GitHub 用户名，必须是这个格式）
4. 其他都保持默认，点最下面的「Create repository」。
5. 进入仓库后，点「uploading an existing file」这个链接，把本文件夹里的所有文件拖进去上传。
6. 等 1~2 分钟，打开 `https://你的用户名.github.io` 就能看到你的网站了。

## 二、怎么写文章

1. 进入你的仓库，打开 `_posts` 文件夹。
2. 点「Add file」→「Create new file」。
3. 文件名填：`2026-08-31-我的第二篇文章.md`（日期和标题随便起，格式是 年-月-日-标题.md）。
4. 文件内容照着 `_posts/2026-08-30-hello-world.md` 的开头写：

```
---
layout: post
title: 我的第二篇文章
date: 2026-08-31
---

这里开始写正文。
```

5. 点「Commit changes」（提交），保存后等一分钟刷新网站就能看到。

## 三、怎么上传文件让别人下载

1. 进入你的仓库，打开 `files` 文件夹。
2. 点「Add file」→「Upload files」，把你想分享的文件拖进去。
3. 点「Commit changes」，文件就会自动出现在网站的「文件」页面上。

## 四、怎么改名字和自我介绍

- 改网站名字、作者名：编辑 `_config.yml` 里的 `title` 和 `author`。
- 改首页自我介绍：编辑 `index.md`。
- 改「关于」页面：编辑 `about.md`。

在 GitHub 网页上点文件 → 点右上角的铅笔图标即可编辑，改完点「Commit changes」保存。
