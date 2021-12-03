---
layout: page
title: Group Members
permalink: /people/
---

<style type="text/css">

.imagebox {
  width: 35%;
  padding-bottom: 0%;
  position: relative;
  float: left;
}
.textbox {
  position: relative;
  width: 95%;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  padding: 250px;
  text-align: justify;
}
</style>


<ul class="photo-gallery">
<div id="wrap">
  {% for person in site.people %}
  <strong>{{ person.name }}, </strong><em>{{ person.title }}</em>
  <div class="entry">
      <div class="imagebox">
        <img width="100%" src="{{ site.baseurl }}/images/{{ person.image }}" alt="{{ person.name}}"/>
      </div>
      <div class="textbox">
        {{ person.content }}
      </div>
  </div>
  <hr>
  <br>
  {% endfor %}
</div>
</ul>
