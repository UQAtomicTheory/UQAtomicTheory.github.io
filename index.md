---
layout: page
---

<img align="right" width="45%" src="{{ site.baseurl }}/images/404.jpg" border="500">

**_Precision Atomic Theory Group, University of Queensland_**
Breif intro to group

### Links
 * link a
 * link b



&nbsp;

*********************************************************************

# Selected publications:

<div class="entry">
{% assign pubs = site.publications | reverse | where:'featured', true %}
{% for pub in pubs limit:6 %}
<article class="post">

  <h1><a href="{{ site.baseurl }}{{ pub.url }}">{{ pub.title }}</a></h1>
  <div class="entry">
    {{ pub.excerpt }}
  </div>

</article>
{% endfor %}
</div>

[See more: /publications:]({{ site.baseurl }}/publications)

*********************************************************************
