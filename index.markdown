---
layout: default
---

<h1>Welcome to The Soulful Sapien</h1>
<p>A digital space to explore ideas, share knowledge, and document a journey of growth.</p>

## Latest Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h3>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
