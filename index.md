# Welcome To My Blog 

Click a post below to read it. 

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} {{ post.category}} ({{ post.date | date: '%B %d, %Y' }})</a>
    </li>
  {% endfor %}
</ul>