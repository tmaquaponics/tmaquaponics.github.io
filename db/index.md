<div class="viewlets">
  {% for fsh in site.fish %}
    <div class="product">
      <div class="product_desc"><p>{{ fsh.title }}</p></div>
      <div class="product_status"><a href="{{ fsh.url }}">view</a></div>
    </div>
  {% endfor %}
</div>
