---
layout: default
title: 博客
permalink: /blog/
description: 关于机器学习、软件工程与持续学习的笔记。
---

<header class="page-hero shell narrow">
  <p class="eyebrow">JOURNAL</p>
  <h1>思考与笔记</h1>
  <p>记录学习过程中的理解、实验和回顾。写下来，是为了把短暂的灵感变成可以反复使用的知识。</p>
</header>

<section class="shell narrow blog-index">
  {% for post in site.posts %}
    <article class="blog-card">
      <p class="post-date">{{ post.date | date: "%Y.%m.%d" }}{% if post.category %} · {{ post.category }}{% endif %}</p>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
      <a class="text-link" href="{{ post.url | relative_url }}">阅读全文 →</a>
    </article>
  {% endfor %}
</section>
