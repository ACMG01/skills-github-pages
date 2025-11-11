# FILE: index.md
---
layout: page
title: Welcome to my blog
permalink: /
---
<div class="hero">
  <div class="hero__content">
    <h1>Level up your GitHub Pages</h1>
    <p class="lead">Short notes, guides, and experiments on development and tools.</p>
    <p>
      <a class="btn" href="{{ '/about/' | relative_url }}">About this site</a>
      <a class="btn btn--secondary" href="{{ '/contact/' | relative_url }}">Contact</a>
    </p>
  </div>
</div>

## Latest posts
<ul class="post-list">
  {%- for post in site.posts limit:5 -%}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {%- endfor -%}
  {%- if site.posts == empty -%}
    <li>No posts yet — create one in <code>_posts/</code>.</li>
  {%- endif -%}
</ul>
