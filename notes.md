---
layout: page
title: Notas
---
{% assign i_notes = site.notes | sort:"date" | reverse %}
<ul>
  {% for note in i_notes %}
    <li>
      <p><a href=".{{ note.url }}">{{ note.title }}</a></p>
    </li>
  {% endfor %}
</ul>