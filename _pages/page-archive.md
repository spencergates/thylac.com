---
title: "Projects"
layout: splash
permalink: /projects/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/color-shredder/d500-q2-c8-opencl-multi.png
  actions:
    - label: "See the Color Shredder"
      url: "/color-shredder/"
excerpt: "Tie-dye pixel art from my latest project."
intro: 
  - excerpt: 'Various Computer Science Projects'

---

{% for post in site.pages %}
  {% if post.featured %}
  <h3>{{post.description}}</h3>
  <a href="{{post.url}}" class="{{post.button}}">{{post.title}}</a>
  {% endif %}
{% endfor %}

