---
layout: default
title: Journal
nav_order: 4
---
 
# Journal
 
{% for post in site.posts %}
 
## [{{ post.title }}{ post.date | date: "%d %b %Y" }}
 
{{ post.excerpt }}
 
---
 
{% endfor %}