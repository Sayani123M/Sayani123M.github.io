---
layout: default
title: "Trading Strategies"
---

<h2>📈 Trading Strategy Posts</h2>

<ul>
  {% for post in site.posts %}
    {% if post.tags contains "trading" %}
      <li>
        <a href="{{ post.url | relative_url }}">
          {{ post.date | date: "%b %-d, %Y" }} &mdash; {{ post.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
