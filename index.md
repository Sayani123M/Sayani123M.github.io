---
layout: default
title: "Probability & Trading Blog"
description: "Dissecting classic puzzles and trading strategies"
---

## Latest Posts

{% if site.posts and site.posts.size > 0 %}
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">
        {{ post.date | date: "%b %-d, %Y" }} &mdash; {{ post.title }}
      </a>
    </li>
  {% endfor %}
</ul>
{% else %}
<p>No posts yet—stay tuned!</p>
{% endif %}
