---
layout: default
title: "Happy Jekylling!"
---

## You're ready to go!

Start developing your Jekyll website.

{% for plant in site.plants  %}
  <h2>{{ plant.name }} - {{ plant.description }}</h2>
  <p>{{ plant.content | markdownify }}</p>
{% endfor %}