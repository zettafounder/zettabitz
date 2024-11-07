---
layout: page
title: Blog
---
<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href=".{{ post.url }}">{{ post.title }}</a></h3>
    </li>
  {% endfor %}
</ul>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>