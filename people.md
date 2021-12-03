---
layout: page
title: Group Members
permalink: /people/
---

<style type="text/css">
#wrap {
  overflow: hidden;
}
.imagebox {
  width: 35%;
  padding-bottom: 0%;
  position: relative;
  float: left;
}
.textbox {
  position: relative;
  left: 25px;
  right: 10px;
  top: 1px;
  bottom: 1px;
  padding: 2px;
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
  <br>
  {% endfor %}
</div>
</ul>
