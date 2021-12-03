---
layout: page
title: People
permalink: /people/
---

People


{% for person in site.people reversed %}
<article class="post">

  <h1><a href="{{ site.baseurl }}{{ person.url }}">{{ person.title }}</a></h1>
  <div class="entry">

  <img src="{{ site.baseurl }}/images/{{ post.image }}">

  {{ person.content }}

  </div>

</article>
{% endfor %}
