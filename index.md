---
title: Sean Parent
tagline: Too many projects, too little time
layout: page
---

## Posts

<ul class="posts">
  {% for post in site.posts %}
    {% if post.category != "draft" %}
      <li>
        <span>{{ post.date | date_to_string }}</span> &raquo;
        <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
