---
layout: resources
title: Crafting
---
{% for category in site.data.categories %}
<section id="{{ category.name }}" class="resources">
{% for crafting in site.data.crafting %}
{% if crafting.category == category.name %}
  <div class="resource">
    <img src="{{crafting.image | prepend: "/assets/images/" | relative_url}}">
    <h3>{{ crafting.name }}</h3>
    <p>{{ crafting.description }}</p>
    <p>Created for BV+<br>Created by {{ crafting.creator }}</p>
  </div>
{% endif %}
{% endfor %}
</section>
{% endfor %}
