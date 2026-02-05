---
layout: default
title: Home
---

# Latest Posts

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncate: 200 }}</p>
  </li>
{% endfor %}
</ul>
