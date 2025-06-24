---
layout: default
title: "Probability Puzzles"
---

<h2>🎲 Probability Puzzle Posts</h2>

<ul>
  {% for post in site.posts %}
    {% if post.tags contains "probability" %}
      <li>
        <a href="{{ post.url | relative_url }}">
          {{ post.date | date: "%b %-d, %Y" }} &mdash; {{ post.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
