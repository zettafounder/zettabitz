# Zetta Bitz Notes

<ul>
  {% for note in notes.android %}
    <li>
      <h3><a href="{{ note.url }}">{{ note.title }}</a></h3>
    </li>
  {% endfor %}
</ul>