---
layout: default
title: Writing
permalink: /writing/
---

# Writing

<ul>
{% for post in site.posts %}
  {% if post.categories contains 'poems' %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date: "%B %d, %Y" }})</li>
  {% endif %}
{% endfor %}
</ul>
