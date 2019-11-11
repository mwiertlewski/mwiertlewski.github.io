---
title: Research
permalink: /research/
---

### Big picture
Our group studies the mechanics linked to tactile perception. Our approach lies at the intersection of the observation of tactile interaction with high precision devices, the design of haptic interfaces for reproducing realistic tactile sensations and the psychophysical study of human perception.


### Projects
<section class="showcase">
<div class="container-fluid p-0">

{% for post in site.posts %}
  {% if post.categories contains 'research' %}
  {% assign odd = forloop.index | modulo:2 %}
  <div class="row no-gutters">
  {% if odd == 0 %}
    <div class="col-lg-6 text-white showcase-img" style="background-image: url('{{site.baseurl}}/images/post/{{post.img}}'); min-height: 15rem;"></div>
    <div class="col-lg-6 my-auto showcase-projects">
      <h3><a href="{{ site.baseurl }}{{ post.url }}" style="color: black;">{{ post.title }}</a></h3>
      <p>{{ post.subtitle }}</p>
    </div>
  {% else %}
    <div class="col-lg-6 my-auto showcase-projects">
      <h3><a href="{{ site.baseurl }}{{ post.url }}" style="color: black;">{{ post.title }}</a></h3>
      <p>{{ post.subtitle }}</p>
    </div>
    <div class="col-lg-6 text-white showcase-img" style="background-image: url('{{site.baseurl}}/images/post/{{post.img}}'); min-height: 15rem;">
    </div>
  {% endif %}  
  </div>
  {% endif %}
{% endfor %}
</div>
</section>
