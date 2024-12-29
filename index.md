---
layout: default
title: "Blog Saya"
---
<link rel="stylesheet" href="/custom.css">
# Selamat datang di Blog Saya!

Di bawah ini adalah daftar posting terbaru saya:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <p>{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
    </li>
  {% endfor %}
</ul>
