---
layout: default
title: Home
---

# Welcome to My Blog

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})

{{ post.excerpt }}

*Posted on {{ post.date | date: "%B %d, %Y" }}*

---
{% endfor %}