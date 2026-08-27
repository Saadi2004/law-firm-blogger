---
layout: default
title: Law Firm Blog
---

## Latest Legal Articles

<ul>
  {% for post in site.posts %}
    <li style="margin-bottom: 25px; list-style: none;">
      {% if post.image %}
        <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" style="max-width: 100%; border-radius: 8px; margin-bottom: 10px;" />
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p><em>{{ post.date | date: "%B %d, %Y" }}</em></p>
      <p>{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>
