---
layout: page
title: People
permalink: /people/
---

People


<!-- {% for person in site.people reversed %}
<article class="post">

  <h1><a href="{{ site.baseurl }}{{ person.url }}">{{ person.name }}</a></h1>
  <div class="entry">

  <img width="33%" src="{{ site.baseurl }}/images/{{ person.image }}" alt="{{ person.name}}" style="float: left"/>
... and ...
  {{ person.content }}

  </div>

</article>
{% endfor %} -->


<style type="text/css">
#wrap {
  overflow: hidden;
}
.imagebox {
  width: 45%;
  padding-bottom: 0%;
  position: relative;
  float: left;
}
.textbox {
  position: relative;
  left: 25px;
  right: 1px;
  top: 1px;
  bottom: 1px;
  padding: 10px;
}
</style>


<ul class="photo-gallery">
<div id="wrap">
  {% for person in site.people %}
  <h1><a href="{{ site.baseurl }}{{ person.url }}">{{ person.name }}</a></h1>
  <h3><a href="{{ site.baseurl }}{{ person.url }}">{{ person.title }}</a></h3>
  <div class="entry">
      <div class="imagebox">
        <img width="100%" src="{{ site.baseurl }}/images/{{ person.image }}" alt="{{ person.name}}"/>
      </div>
      <div class="textbox">
        {{ person.content }}
      </div>
  </div>
  {% endfor %}
</div>
</ul>
