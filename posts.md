---
layout: default
title: Beiträge
permalink: /posts/
body-class: posts-page
---

<div class="posts-wrapper">
  <h1>Alle Blogeinträge</h1>
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a> –
        <span>{{ post.date | date: "%d.%m.%Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</div>