---
layout: page
title: Welcome
tagline: 
---
{% include JB/setup %}
    
## Rescent Posts


<ul class="posts">
  {% for post in site.posts %}
<li><span class='date'>{{ post.date | date: "%B %e, %Y" }}</span><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
<span class='slug'>{{ post.content | strip_html | truncatewords : 100 }}...</span>

</li>
  {% endfor %}
</ul>

## Tags
<ul class="tag_box inline">
  {% assign tags_list = site.tags %}
  {% include JB/tags_list %}
</ul>

