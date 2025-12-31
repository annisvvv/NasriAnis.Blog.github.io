---
layout: page
title: ""
---

#### Welcome to my blog

This is my personal blog i wish i could help someone of you get inspired, wish you  good lecture.

### Posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      - <span>{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>