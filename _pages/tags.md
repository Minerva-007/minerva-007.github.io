---
layout: single
permalink: /tags
title: "Tags"
header:
   overlay_image: /assets/images/DigitalTwin.png
   show_overlay_excerpt: true
   overlay_filter: 0.5
   caption: "A Digital Twin of a speed and position controlled trolley system"
excerpt: All posts, sorted by tags.
---

{% for tag in site.tags %}
  <h1>{{ tag[0] }}</h1>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
