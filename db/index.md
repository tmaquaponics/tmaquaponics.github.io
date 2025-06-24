<div class="viewlets">
  {% for fsh in site.fish %}
    <div class="product">
      <div class="product_desc"><p>{{ fsh.title }}</p></div>
      <div class="product_image"><a href="{{ fsh.url }}"><img src="![Gold dust molly](/assets/img/1739103569781.jpg)" /></a></div>
      <div class="product_status"></div>
    </div>
  {% endfor %}
</div>
