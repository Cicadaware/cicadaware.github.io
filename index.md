---
layout: default
title: Home
---

<div class="post-grid">
    {% for post in site.posts %}
        <a href="{{ post.url }}" class="post-link">
        <div class="post-block">
            <h2>{{ post.title }}</h2>
            <p>{{ post.excerpt }}</p>   
            <p>{{ post.summary }}</p>
            <p><small> Posted on {{ post.date | date: "%B %d, %Y" }} </small></p>
        </div>
        </a>
    {% endfor %}
</div>