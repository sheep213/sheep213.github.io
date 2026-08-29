---
layout: default
title: 留言
permalink: /message/
---

# 给我留言

有什么想对我说的，在这里写下来。你的留言会**悄悄发到我的邮箱**，只有我看得到，不会在网站上公开。

<form class="message-form" action="https://formsubmit.co/1797005516@qq.com" method="POST">
  <input type="hidden" name="_subject" value="网站新留言">
  <input type="hidden" name="_template" value="table">
  <input type="text" name="_honey" style="display:none">

  <label for="name">你的称呼（选填）</label>
  <input type="text" id="name" name="称呼">

  <label for="content">留言内容</label>
  <textarea id="content" name="留言内容" rows="5" required></textarea>

  <button type="submit">发送留言</button>
</form>
