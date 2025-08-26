---
layout: default
title: Blog
permalink: /blog/
---

<h1>{{ page.title }}</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>— {{ post.date | date: "%B %d, %Y" }}</small>
      {% if post.excerpt %}<div>{{ post.excerpt | strip_html | truncate: 140 }}</div>{% endif %}
    </li>
  {% endfor %}
</ul>