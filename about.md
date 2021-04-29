---
layout: main
title: "About"
---
<h1>Members of Bedrock Vanilla +</h1>
<section class="staff">
{% for staff_member in site.staff_members %}
  <div class="member">
    <img class="avatar" src="{{staff_member.name | prepend: "/assets/images/avatars/" | append: "-logo.png" | relative_url }}">
    <h4>{{ staff_member.name }}</h4>
    {% if staff_member.discord %}
    <a href="{{"https://discord.com/invite/" | append: staff_member.discord }}" target="_BLANK"><img src="{{"discord-logo.png" | prepend: "/assets/images/" | relative_url }}"></a>
    {% endif %}
    {% if staff_member.youtube %}
    <a href="{{"http://youtube.com/" | append: staff_member.youtube }}" target="_BLANK"><img src="{{"youtube-logo.png" | prepend: "/assets/images/" | relative_url }}"></a>
    {% endif %}
    {% if staff_member.twitch %}
    <a href="{{"http://twitch.tv/" | append: staff_member.twitch }}" target="_BLANK"><img src="{{"twitch-logo.png" | prepend: "/assets/images/" | relative_url }}"></a>
    {% endif %}
    {% if staff_member.patreon %}
    <a href="{{"http://patreon.com/" | append: staff_member.patreon }}" target="_BLANK"><img src="{{"patreon-logo.png" | prepend: "/assets/images/" | relative_url }}"></a>
    {% endif %}
  </div>
{% endfor %}
<section>
