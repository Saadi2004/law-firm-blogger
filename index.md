---
layout: default
title: Law Firm Blog
---

## Latest Legal Articles

<ul>
  {% for post in site.posts %}
    <li style="margin-bottom: 20px;">
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
      <p><em>{{ post.date | date: "%B %d, %Y" }}</em></p>
      <p>{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>
