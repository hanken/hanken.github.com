---
layout: page
title: Home
tagline: 
---
{% include JB/setup %}
    
### Rescent Posts


<ul class="posts">
  {% for post in site.posts %}
    <li><span class='date'>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>

<span class='slug'>{{ post.content | strip_html | truncatewords : 100 }}...</span>
</li>
  {% endfor %}
</ul>


