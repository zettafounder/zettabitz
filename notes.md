---
layout: page
title: Notas
---
<ul>
  {% for note in site.notes | reverse %}
    <li>
      <h4><a href=".{{ note.url }}">{{ note.title }}</a></h4>
    </li>
  {% endfor %}
</ul>