---
title: My personal Blog
layout: "base.njk"
---

Hello Welcome to my Blog.

<ul>
{%- for post in collections.all -%}
  <li><a href="{{ post.url }}">{{ post.url }}</a></li>
{%- endfor -%}
</ul>
