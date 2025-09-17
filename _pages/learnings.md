---
layout: collection
permalink: /learnings/
---

My awesome learning journey...

{% assign sorted_learnings = site.learnings | sort: 'end_date' | reverse %}

<table>
<tr>
  <th>
    When
  </th>
  <th>
    What
  </th>
  <th>
    Where
  </th>
</tr>
  {% for learning in sorted_learnings %}
    <tr>
      <td style="white-space: nowrap;"> {{ learning.end_date | date: "%Y" }} </td>
      <td style="white-space: nowrap;"> {{ learning.title }} </td>
      <td style="white-space: nowrap;"> {{ learning.board }}, {{ learning.location }} </td>
    </tr>
  {% endfor %}
</table>
