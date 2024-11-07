---
layout: page
title: Blog
---
<ul>
  {% for post in site.posts %}
    <li>
      <h4>post.datee<a href=".{{ post.url }}">{{ post.title }}</a></h4>
    </li>
  {% endfor %}
</ul>