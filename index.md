# Zetta Bitz Notes

## Blog

<h1>Ultimas entradas</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="zettabitz/{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>