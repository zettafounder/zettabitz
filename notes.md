---
layout: page
title: Notas
---
{% assign i_notes = site.notes | sort:"date" | reverse %}
<ul>
  {% for note in i_notes %}
    <li>
      <h4><a href=".{{ note.url }}">{{ note.title }}</a></h4>
    </li>
  {% endfor %}
</ul>