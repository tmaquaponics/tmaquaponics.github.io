---
layout: default
title: Blog archive
---

<ul><li><a href="{{ site.url }}">Back</a></li></ul>

### All Posts

<ul>
  {% for post in site.posts %}
    <li>
      {{ post.date | date_to_string }} <a href="{{ post.url }}">{{ post.title }}</a> 
    </li>
  {% endfor %}
</ul>
