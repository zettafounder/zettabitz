---
layout: page
title: Notas
---
{% assign i_notes = site.notes | sort:"date" | reverse %}
{% for note in i_notes %}
  <div>&raquo; <a href=".{{ note.url }}"><strong>{{ note.title }}</strong></a></div>
{% endfor %}