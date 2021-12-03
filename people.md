---
layout: page
title: People
permalink: /people/
---

People


{% for person in site.people reversed %}
<article class="post">

  <h1><a href="{{ site.baseurl }}{{ person.url }}">{{ person.name }}</a></h1>
  <div class="entry">

  <img src="{{ site.baseurl }}/images/{{ person.image }}">

  {{ person.content }}

  </div>

</article>
{% endfor %}


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
  width: 50%;
  padding-bottom: 85%;
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
  position: absolute;
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
    <div class="longbox">
      <div class="innerContent">
        <img width="100%" src="{{ site.baseurl }}/images/{{ person.image }}" alt="{{ person.name}}"/>
      </div>
      <div class="innerContent">
        {{ person.content }}
      </div>
    </div>
  {% endfor %}
</div>
</ul>
