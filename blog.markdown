---
title: blog
date: 2020-06-04 18:15:00 Z
author: Janvier Byiringiro
layout: default
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>

      <hr/>
      <p> {{post.content}} </p>
    </li>
  {% endfor %}
</ul>
