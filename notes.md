---
layout: page
title: Notes
---
<ul>
  {% for note in site.notes %}
    <li>
      <h3><a href=".{{ note.url }}">{{ note.title }}</a></h3>
    </li>
  {% endfor %}
</ul>