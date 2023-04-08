---
title: Zines
layout: collection
permalink: /zines/
collection: zines
entries_layout: list
author_profile: true
classes: wide
header:
    overlay_image: /assets/images/banner1.png
    overlay_filter: linear-gradient(to right, rgba(0, 120, 220, 1), rgba(0, 0, 0,.1))
---
{% for zine in site.collections.zines %}
  <div class="zine">
    <h2>{{ zine.title }}</h2>
    <img src="{{ zine.teaser }}" alt="{{ zine.title }} teaser">
    <p>{{ zine.excerpt }}</p>
  </div>
{% endfor %}