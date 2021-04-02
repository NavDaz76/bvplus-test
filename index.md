---
layout: main
title: "Main"
---
<main>
  <div class="wrapper">
    <section class="category-navigation">
    Show the tabs for different categories here!
    </section>
    <section class="resources">
      {% for resources in site.data.resources %}
        <div class="resource">
          <img src="{{ "/assets/images/"}}{{resources.image }}">
          <h3>{{ resources.name }}</h3>
          <p>Created for BV+<br>Created by {{ resources.creator }}</p>
          </div>
          {% endfor %}
    </section>
    <section class="other-stuff">
      This is for other stuff
    </section>
  </div>
</main>
