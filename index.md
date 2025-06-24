---
layout: default
title: "Probability & Trading Blog"
description: "Dissecting classic puzzles and trading strategies"
---

<h1 style="text-align:center;">Welcome to my Quantitative Blog 🧠📊</h1>
<p style="text-align:center;">Explore insights into probability puzzles and trading strategies.</p>

<div style="display: flex; justify-content: center; gap: 40px; margin: 30px 0;">
  <a href="/tag/probability" style="text-decoration: none;">
    <div style="background-color: #f0f0f0; padding: 20px 40px; border-radius: 10px; text-align: center; box-shadow: 2px 2px 8px rgba(0,0,0,0.2);">
      <h2>🎲 Probability Puzzles</h2>
      <p>Explore logic puzzles and paradoxes.</p>
    </div>
  </a>
  <a href="/tag/trading" style="text-decoration: none;">
    <div style="background-color: #f0f0f0; padding: 20px 40px; border-radius: 10px; text-align: center; box-shadow: 2px 2px 8px rgba(0,0,0,0.2);">
      <h2>📈 Trading Strategies</h2>
      <p>Explore backtests and crypto strategies.</p>
    </div>
  </a>
</div>

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
