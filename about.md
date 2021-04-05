---
layout: main
title: "About"
---
<h1>Members of Bedrock Vanilla +</h1>
{% for staff_member in site.staff_members %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
