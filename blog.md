---
layout: page
title: Blog
---
{% for post in site.posts %}
  <div>{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    <time class="dt-published" datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">
      {{ post.date | date: date_format }}
    </time>
    {%- if post.modified_date -%}
      ~ 
      {%- assign mdate = post.modified_date | date_to_xmlschema -%}
      <time class="dt-modified" datetime="{{ mdate }}" itemprop="dateModified">
        {{ mdate | date: date_format }}
      </time>
    {%- endif -%} - <a href=".{{ post.url }}"><strong>{{ post.title }}</strong></a></div> 
{% endfor %}

<a rel="me" href="https://zettafounder.github.io/zettabitz/feed.xml">RSS</a>