---
layout: page
---

|<img align="right" width="45%" src="{{ site.baseurl }}/images/group.jpg">|
-

**Precision Atomic Theory Group**
**_University of Queensland, Australia_**

Some background info about group. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.


### Research Areas
  * High-precision atomic many-body theory
  * Quantum electrodynamics corrections to heavy-atom phenomena
  * Violations of fundamental symmetries
  * Precision tests of the standard model of particle physics and searches for new physics
  * Superheavy elements
  * Searches for dark matter and exotic physics
  * Particle astrophysics


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

[See more: /research:]({{ site.baseurl }}/publications)

*********************************************************************
