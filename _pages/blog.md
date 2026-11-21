---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

{% include base_path %}

{% if site.posts.size > 0 %}
<div class="blog-list">
{% for post in site.posts %}
  <div class="blog-item">
    <div class="blog-date">{{ post.date | date: "%b %d, %Y" }}</div>
    <div class="blog-main">
      <a class="blog-title" href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
      {% if post.excerpt %}<div class="blog-excerpt">{{ post.excerpt | strip_html | truncatewords: 40 }}</div>{% endif %}
    </div>
  </div>
{% endfor %}
</div>
{% else %}
<p class="blog-empty">No posts yet. Write-ups on my research and things I find interesting will appear here soon.</p>
{% endif %}

<style>
.blog-empty {
  margin-top: 1em;
  color: var(--global-text-color-light);
  font-style: italic;
}
.blog-item {
  display: flex;
  gap: 16px;
  align-items: baseline;
  padding: 12px 0;
  border-bottom: 1px solid var(--global-border-color);
}
.blog-item:last-child { border-bottom: none; }
.blog-date {
  flex-shrink: 0;
  width: 100px;
  font-family: "Inter", -apple-system, sans-serif;
  font-size: 0.8em;
  font-weight: 600;
  color: var(--global-text-color-light);
}
.blog-main { flex: 1; min-width: 0; }
.blog-title {
  font-family: "Inter", -apple-system, sans-serif;
  font-weight: 600;
  color: var(--global-text-color);
  text-decoration: none;
}
.blog-title:hover { color: var(--global-link-color); text-decoration: underline; }
.blog-excerpt { margin-top: 4px; font-size: 0.9em; color: var(--global-text-color-light); }
@media (max-width: 480px) {
  .blog-item { flex-direction: column; gap: 2px; }
}
</style>
