---
layout: default
title: My Projects
---

# Featured Projects

Here is a collection of my work in data science, numerical analysis, and statistics.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a> — 
      {{ post.date | date: "%B %d, %Y" }}
      <p>{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
    </li>
  {% endfor %}
</ul>
