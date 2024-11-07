# Zetta Bitz Notes

<ul>
  {% for note in site.notes %}
    <li>
      <h3><a href="{{ zettabitz/ }}{{ note.url }}">{{ note.title }}</a></h3>
    </li>
  {% endfor %}
</ul>