---
layout: page
title: Notes
---
<ul>
  {% for note in site.notes %}
    <li>
      <h4><a href=".{{ note.url }}">{{ note.title }}</a></h4>
    </li>
  {% endfor %}
</ul>