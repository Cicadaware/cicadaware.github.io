---
layout: default
title: Home
---

<p>Number of posts: {{ site.posts | size }}</p>

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
<div class="post-block">
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>

<p>{{ post.exerpt }}</p>

<p>{{ post.summary }}</p>

*Posted on {{ post.date | date: "%B %d, %Y" }}*

</div>
{% endfor %}
