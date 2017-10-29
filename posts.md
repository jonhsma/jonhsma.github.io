---
bg: "vancouver.jpg"
layout: page
title: "Posts"
crawlertitle: "Posts"
permalink: /posts/
summary: "Thoughs and News"
active: posts
---

{% for post in site.posts limit: 5 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
