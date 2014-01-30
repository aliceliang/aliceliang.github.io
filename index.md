---
layout: default
title: aliceliang
---

<h1> notes </h1>
<ul class="posts">
  {% for post in site.posts %}
    {% if post.tags contains "commentary" %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
