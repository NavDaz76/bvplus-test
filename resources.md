---
layout: resources
title: "Resources"
---
{% for resources in site.data.resources %}
  <div class="resource">
    <img src="{{resources.image | prepend: "/assets/images/" | relative_url}}">
    <h3>{{ resources.name }}</h3>
    <p>Created for BV+<br>Created by {{ resources.creator }}</p>
  </div>
{% endfor %}
