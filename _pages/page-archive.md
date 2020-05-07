---
title: "Projects"
layout: splash
permalink: /projects/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/d500-q2-c8-opencl-multi.png
  actions:
    - label: "See the Color Shredder"
      url: "/color-shredder/"
excerpt: "Tie-dye pixel art from my latest project."
intro: 
  - excerpt: 'Various Computer Science Projects'

---




{% for post in site.pages %}
  {% if post.featured %}
  <h1>{{post.description}}</h1>
  <a href="{{post.url}}" class="btn btn--primary btn--x-large">{{post.title}}</a>
  {% endif %}
{% endfor %}

