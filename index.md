---
layout: default
title: Tank-Mates Aquaponics
---

Welcome to the Tank-Mates Aquaponics website. We provide a variety of products which you can find in the shop section. 
You can also find all our posts below. For business inquiries you can reach us at <strong>tankmatesaquaponics@gmail.com</strong>. 

### All Posts

<ul>
  {% for post in site.posts %}
    <li>
      {{ post.date | date_to_string }} <a href="{{ post.url }}">{{ post.title }}</a> 
    </li>
  {% endfor %}
</ul>
