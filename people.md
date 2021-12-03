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

  <img width="33%" src="{{ site.baseurl }}/images/{{ person.image }}" alt="{{ person.name}}" style="float: left"/>
... and ...
  {{ person.content }}

  </div>

</article>
{% endfor %}
