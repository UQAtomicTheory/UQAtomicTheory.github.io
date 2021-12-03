---
layout: page
title: Recent publications
permalink: /publications/
---

{% for pub in site.publications reversed %}
 <article class="post">

   <h1><a href="{{ site.baseurl }}{{ pub.url }}">{{ pub.title }}</a></h1>
   <div class="entry">
     {{ pub.excerpt }}
   </div>

 </article>
 {% endfor %}
