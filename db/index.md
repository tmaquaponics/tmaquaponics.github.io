<div class="viewlets">
  {% for fsh in site.fish %}
    <div class="product">
      <div class="product_image"><a href="{{ fsh.url }}"><img src="/assets/img/1739103569781.jpg" /></a></div>
      <div class="product_status"><span>{{ fsh.title }}</span></div>
    </div>
  {% endfor %}
</div>
