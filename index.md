---
layout: default
title: "Happy Jekylling!"
---
<center>
  <header class="header">
    <h1>MON PETIT JARDIN</h1>
  </header>

  {% for plant in site.plants  %}
    <div class="wrapper-card">
      <div class="card">
        <a href="{{ plant.url }}">
          <img class="card-picture" src="{{plant.picture}}">
        </a>
      </div>
      <div class='card-name'>
        <p class="plant-name">
          {{plant.name}}
        </p>
      </div>
    </div>
  {% endfor %}
</center>