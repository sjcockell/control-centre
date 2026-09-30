---
layout: default
title: Journal
nav_order: 4
---
 
# Journal
 
{% for post in site.posts %}
 
<a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%d %b %Y" }}</a>
 
{{ post.excerpt }}
 
---
 
{% endfor %}