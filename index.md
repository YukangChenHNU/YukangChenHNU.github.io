---
layout: default
title:
description: Yukang Chen 的个人主页
---

<section class="hero shell">
  <div class="hero-copy">
    <h1>Yukang Chen<br><span>陈裕康</span></h1>
    <p class="hero-lead">第一次建立个人主页</p>
    <div class="hero-actions">
      <a class="button primary" href="{{ '/projects/' | relative_url }}">浏览项目</a>
      <a class="button secondary" href="{{ '/blog/' | relative_url }}">阅读博客</a>
    </div>
  </div>
  <div class="hero-card" aria-label="个人简介">
    <div class="portrait">
      <img src="https://github.com/YukangChenHNU.png?size=320" alt="Yukang Chen 的 GitHub 头像">
    </div>
    <div class="status"><span></span> Open to learning & collaboration</div>
    <dl>
      <div><dt>方向</dt><dd>Machine Learning</dd></div>
      <div><dt>关注</dt><dd>Algorithms · Engineering</dd></div>
      <div><dt>坐标</dt><dd>Hunan, China</dd></div>
    </dl>
  </div>
</section>

<section class="section shell">
  <div class="section-heading">
    <div><p class="eyebrow">SELECTED WORK</p><h2>精选项目</h2></div>
    <a class="text-link" href="{{ '/projects/' | relative_url }}">查看全部 →</a>
  </div>
  <div class="project-grid">
    <article class="project-card featured">
      <div class="project-number">01</div>
      <div>
        <div class="tags"><span>Python</span><span>Machine Learning</span></div>
        <h3>Machine Learning from Scratch</h3>
        <p>不依赖高级机器学习框架，从零实现经典算法，在实践中理解模型背后的数学与工程细节。</p>
        <a class="card-link" href="https://github.com/YukangChenHNU/Machine-Learning-from-Scratch" target="_blank" rel="noopener">查看源码 ↗</a>
      </div>
    </article>
    <article class="project-card quiet-card">
      <div class="project-number">02</div>
      <div>
        <div class="tags"><span>Portfolio</span><span>Jekyll</span></div>
        <h3>Personal Knowledge Garden</h3>
        <p>这个网站本身也是持续迭代的项目：整理项目、记录思考，让零散知识形成长期积累。</p>
        <a class="card-link" href="{{ '/blog/' | relative_url }}">浏览文章 →</a>
      </div>
    </article>
  </div>
</section>

<section class="section shell">
  <div class="section-heading">
    <div><p class="eyebrow">RECENT NOTES</p><h2>最近文章</h2></div>
    <a class="text-link" href="{{ '/blog/' | relative_url }}">全部文章 →</a>
  </div>
  <div class="post-list">
    {% for post in site.posts limit: 3 %}
      <a class="post-row" href="{{ post.url | relative_url }}">
        <span class="post-date">{{ post.date | date: "%Y.%m.%d" }}</span>
        <span class="post-title">{{ post.title }}</span>
        <span class="post-arrow">↗</span>
      </a>
    {% endfor %}
  </div>
</section>

<section class="closing shell">
  <p class="eyebrow">LET’S CONNECT</p>
  <h2>让想法落地，<br>也让知识留下痕迹。</h2>
  <a class="button primary" href="https://github.com/YukangChenHNU" target="_blank" rel="noopener">在 GitHub 找到我 ↗</a>
</section>
