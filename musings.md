---
layout: default
title: Musings
permalink: /musings/
---

# Musings

<ul>
{% for post in site.posts %}
  {% if post.categories contains 'musings' %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date: "%B %d, %Y" }})</li>
  {% endif %}
{% endfor %}
</ul>
