<div class="viewlets">



<ul>
  {% for fsh in site.fish %}
    <li>
      <a href="{{ fsh.url }}">{{ fsh.title }}</a> 
    </li>
  {% endfor %}
</ul>
 
</div>
