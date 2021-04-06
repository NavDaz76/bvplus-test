---
layout: resources
title: "Resources"
---
{% for category in site.data.categories %}
<section id="{{ category.name }}" class="resources">
{% for resources in site.data.resources %}
{% if resources.category == category.name %}
  <div class="resource">
    <img src="{{resources.image | prepend: "/assets/images/" | relative_url}}">
    <h3>{{ resources.name }}</h3>
    <p>Created for BV+<br>Created by {{ resources.creator }}</p>
  </div>
{% endif %}
{% endfor %}
</section>
{% endfor %}
