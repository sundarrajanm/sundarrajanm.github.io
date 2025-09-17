---
layout: collection
permalink: /experiences/
---

Below is a detailed summary of my professional experience across various organizations:

{% assign sorted_experiences = site.experiences | sort: 'start_date' | reverse %}

<table>
<tr>
  <th>
    Started
  </th>
  <th>
    Role
  </th>
  <th>
    Organisation
  </th>
  <th>
    Location
  </th>
</tr>
  {% for experience in sorted_experiences %}
    <tr>
      <td> {{ experience.start_date | date: "%b %Y" }} </td>
      <td> {{ experience.role }} </td>
      <td> <a href="{{ experience.url }}">{{ experience.title }}</a> </td>
      <td> {{ experience.location }} </td>
    </tr>
  {% endfor %}
</table>
