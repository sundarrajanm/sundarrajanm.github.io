---
title: "Experiences"
layout: collection
permalink: /experiences/
---

Here’s a summary of my professional experience across various organizations:

{% assign sorted_experiences = site.experiences | sort: 'start_date' | reverse %}
<ul>
  {% for experience in sorted_experiences %}
    <li><a href="{{ experience.url }}">{{ experience.title }} - {{ experience.start_date | date: "%b %Y" }}</a></li>
  {% endfor %}
</ul>
