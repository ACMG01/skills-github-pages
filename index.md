---
layout: page
title: Welcome to my blog
permalink: /
---
<section class="hero hero--gradient">
  <div class="hero__content">
    <h1 class="display">Welcome to my blog</h1>
    <p class="lead">Level up your GitHub Pages. Short notes, guides, and experiments on development and tools.</p>
    <p class="btn-row">
      <a class="btn" href="{{ '/about/' | relative_url }}">About this site</a>
      <a class="btn btn--ghost" href="{{ '/support/' | relative_url }}">Support us</a>
    </p>
  </div>
</section>

<section class="section">
  <h2 class="section__title">What you’ll find here</h2>
  <div class="grid grid-3">
    <article class="card lift">
      <div class="card__icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M3 5h18v2H3zM3 11h18v2H3zM3 17h18v2H3z"/></svg>
      </div>
      <h3>Concise Guides</h3>
      <p>Step-by-step notes you can skim and apply immediately.</p>
    </article>
    <article class="card lift">
      <div class="card__icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M12 2l4 7 8 1-6 5 2 8-8-4-8 4 2-8-6-5 8-1z"/></svg>
      </div>
      <h3>Practical Patterns</h3>
      <p>Copy-paste snippets for everyday dev tasks.</p>
    </article>
    <article class="card lift">
      <div class="card__icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M4 4h16v4H4zM4 10h10v10H4zM16 10h4v10h-4z"/></svg>
      </div>
      <h3>Minimal Setup</h3>
      <p>No heavy frameworks; just Jekyll + clean CSS.</p>
    </article>
  </div>
</section>

<section class="section">
  <h2 class="section__title">Latest posts</h2>
  <ul class="post-cards">
    {%- for post in site.posts limit:6 -%}
    <li class="post-card lift">
      <a class="post-card__link" href="{{ post.url | relative_url }}">
        <span class="post-card__date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <span class="post-card__title">{{ post.title }}</span>
        <span class="post-card__chevron" aria-hidden="true">→</span>
      </a>
    </li>
    {%- endfor -%}
    {%- if site.posts == empty -%}
      <li>No posts yet — create one in <code>_posts/</code>.</li>
    {%- endif -%}
  </ul>
</section>

<section class="cta">
  <h2>Enjoying the content?</h2>
  <p>Help keep it running. Every bit of support means more tutorials.</p>
  <a class="btn" href="{{ '/support/' | relative_url }}">Support us</a>
</section>

