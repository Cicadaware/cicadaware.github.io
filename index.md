---
layout: default
title: Home
---

# Welcome to My Blog

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
    <small>Posted on {{ post.date | date: "%B %d, %Y" }}</small>
  </article>
{% endfor %}