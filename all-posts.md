---
layout: page
title: All posts
---

{% for post in site.posts %}
{% if post.categories contains "running" %}
{% else %}
  <a href="{{ post.url }}">{{ post.title }}</a> <small>{{ post.date | date_to_string }}</small>
{% endif %}
{% endfor %}