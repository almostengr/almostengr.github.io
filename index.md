---
title: Welcome To My Blog
---

Click a post below to read it.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} ({{ post.date | date: '%B %d, %Y' }})</a>
      {% if post.category != null %}
        [{{ post.category }}] 
      {% elsif post.categories != null %}
        [{{ post.categories }}] 
      {% endif %} 
    </li>
  {% endfor %}
</ul>