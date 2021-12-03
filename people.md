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
.box {
  width: 50%;
  padding-bottom: 50%;
  position: relative;
  float: left;
}
.longbox {
  width: 30%;
  padding-bottom: 30%;
  position: relative;
  float: left;
}
.bigbox {
  width: 100%;
  padding-bottom: 100%;
  position: relative;
  float: left;
}
.innerContent {
  position: relative;
  left: 1px;
  right: 1px;
  top: 1px;
  bottom: 1px;
  padding: 10px;
}
</style>


<ul class="photo-gallery">
<div id="wrap">
  {% for person in site.people %}
    <div class="bigbox">
      <div class="longbox">
        <img width="100%" src="{{ site.baseurl }}/images/{{ person.image }}" alt="{{ person.name}}"/>
      </div>
      <div class="innerContent">
        {{ person.content }}
      </div>
    </div>
  {% endfor %}
</div>
</ul>
