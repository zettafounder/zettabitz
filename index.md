## Blog
<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href=".{{ post.url }}">{{ post.title }}</a></h3>
    </li>
  {% endfor %}
</ul>

## Notas
<ul>
  {% for note in site.notes %}
    <li>
      <h3><a href=".{{ note.url }}">{{ note.title }}</a></h3>
    </li>
  {% endfor %}
</ul>