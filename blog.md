---
layout: page
title: My Posts
permalink: /blog/
---

### All My Writings

<ul class="post-list">
  {% assign sorted_posts = site.posts | sort: 'date' | reverse %}
  {% for post in sorted_posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title }}
        </a>
      </h3>
    </li>
  {% endfor %}
</ul>