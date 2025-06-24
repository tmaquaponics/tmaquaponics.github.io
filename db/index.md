<div class="viewlets">
  {% for fsh in site.fish %}
    <div class="product">
      <div class="product_image"><a href="{{ fsh.url }}"><img src="/assets/img/{{fsh.image}}" /></a></div>
      <div class="product_status"><span>{{ fsh.title }}</span></div>
    </div>
  {% endfor %}
</div>
