# Welcome To My Blog

Click a post below to read it.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
        {% if post.category != null &}
          [{{ post.category}}] 
        {% endif %} 
        ({{ post.date | date: '%B %d, %Y' }})
    </li>
  {% endfor %}
</ul>