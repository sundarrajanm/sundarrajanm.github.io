---
title: "Experiences"
layout: collection
permalink: /experiences/
---

Here’s a summary of my professional experience across various organizations:

{% assign sorted_experiences = site.experiences %}
<ul>
  {% for experience in site.experiences %}
    <li><a href="{{ experience.url }}">{{ experience.title }}</a></li>
  {% endfor %}
</ul>
