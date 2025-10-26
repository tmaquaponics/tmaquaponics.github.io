---
layout: default
title: Tank-Mates Aquaponics
---

Welcome to the Tank-Mates Aquaponics website. A website about fishkeeping and aquaponics.
You can find all our posts below. For business inquiries you can reach us at <strong>tankmatesaquaponics@gmail.com</strong>. 

### All Posts

<ul>
  {% for post in site.posts %}
    <li>
      {{ post.date | date_to_string }} <a href="{{ post.url }}">{{ post.title }}</a> 
    </li>
  {% endfor %}
</ul>
