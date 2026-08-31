---
title: "GeGRAV@UFABC"
layout: homelay
excerpt: "GeGRAV at UFABC."
sitemap: false
permalink: /
---
<div class="page-header">
<h1>
GeGRAV @ UAFBC<br>
<small>Exploring gravity, from black holes to the cosmos</small>
</h1>
</div>

<div markdown="0" id="home-carousel" class="carousel slide" data-ride="carousel" data-interval="10000" data-pause="null" data-keyboard="true" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        {% assign slide_number = 0 %}
        {% for image in site.data.home-carousel %}
        {% if slide_number == 0 %}
            <li data-target="#home-carousel" data-slide-to="{{ slide_number }}" class="active"></li>
        {% else %}
        <li data-target="#home-carousel" data-slide-to="{{ slide_number }}"></li>
        {% endif %}
        {% assign slide_number = slide_number | plus: 1 %}
        {% endfor %}
    </ol>
    <!-- Items -->
    <div class="carousel-inner">
    {% assign slide_number = 0 %}
    {% for image in site.data.home-carousel %}

        {% if slide_number == 0 %}
            <div class="item active">
        {% else %}
            <div class="item">
        {% endif %}
            <img src="{{ site.url }}{{ site.baseurl }}/images/{{ image.image }}" alt="Slide {{ slide_number }}" />
        </div>

    {% assign slide_number = slide_number | plus: 1 %}
    {% endfor %}
    </div>
  <a class="left carousel-control" href="#home-carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#home-carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>
<div align="justify">
<p class="lead"><a href="/research/">Research</a> in the Gravitation Study Group (Grupo de Estudo em Gravitação - GeGRAV) is dedicated to exploring the fundamental principles of Einstein’s theory of General Relativity and its astrophysical applications. Through regular seminars and collaborative discussions, we investigate topics ranging from black hole physics to gravitational waves and cosmology. Our mission is to foster deep understanding, critical thinking, and scientific exchange among students and researchers alike. 
   <!-- <a href="/bec/">first Belgian lab hosting a Bose-Einstein Condensate</a>.</p> -->
</div>
