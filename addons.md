---
layout: resources
title: Add-Ons
---
{% for category in site.data.categories %}
<section id="{{ category.name }}" class="resources">
{% for addon in site.data.addons %}
{% if addon.category == category.name %}
  <div class="resource">
    <img src="{{addon.image | prepend: "/assets/images/" | relative_url}}">
    <h3>{{ addon.name }}</h3>
    <p>Created for BV+<br>Created by {{ addon.creator }}</p>
  </div>
{% endif %}
{% endfor %}
</section>
{% endfor %}
