---
layout: page
title: Posts
permalink: /posts/
---

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <time>{{ post.date | date: "%B %d, %Y" }}</time>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}