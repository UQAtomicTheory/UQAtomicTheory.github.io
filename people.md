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
    {{ person.content }}
    {{ person.image }}
  </div>

</article>
{% endfor %}
