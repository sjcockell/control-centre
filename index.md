---
layout: default
title: Dashboard
nav_order: 1
---

# Dashboard

<div class="dashboard-grid">

<!-- TEACHING LINKS -->
<div class="dashboard-card">
<h2><i class="fa-solid fa-graduation-cap"></i> Teaching</h2>
{% for item in site.data.bookmarks.teaching %}
<a href="{{ item.url }}" class="btn"  target="_blank"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}
</div>

<!-- CANVAS -->
<div class="dashboard-card">
<h2><i class="fa-brands fa-empire"></i> Canvas</h2>
{% for item in site.data.bookmarks.modules %}
<a href="{{ item.url }}" class="btn"  target="_blank"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}
</div>

<!-- UNIVERSITY SERVICES -->
<div class="dashboard-card">
<h2><i class="fa-solid fa-institution"></i> University Services</h2>
{% for item in site.data.bookmarks.university %}
<a href="{{ item.url }}" class="btn"  target="_blank"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}
</div>

<!-- RESEARCH LINKS -->
<div class="dashboard-card">
<h2><i class="fa-solid fa-microscope"></i> Research</h2>

{% for item in site.data.bookmarks.research %}
<a href="{{ item.url }}" class="btn"  target="_blank"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}

</div>

<!-- JOURNAL -->
<div class="dashboard-card">
<h2><i class="fa-solid fa-book"></i> Journal</h2>

{% for post in site.posts limit:5 %}

<i class="fa-solid fa-circle-right"></i> <a href="{{ post.url | relative_url }}">{{ post.date | date: "%d %b" }} - {{ post.title }}</a>
<br/>

{% endfor %}

</div>

<!-- TASKS -->
<div class="dashboard-card">
<h2><i class="fa-solid fa-square-check"></i> Tasks</h2>

{% for item in site.data.bookmarks.tasks %}
<a href="{{ item.url }}" class="btn" target="_blank"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}

</div>

<!-- PROJECTS -->
<div class="dashboard-card dashboard-wide">
<h2>🚀 Current Projects</h2>

<ul>
<li>First-Year Seminar Development</li>
<li>Bioinformatics Practical Redesign</li>
<li>Single-cell Teaching Resources</li>
</ul>

</div>

<!-- RECENTLY UPDATED -->
<div class="dashboard-card dashboard-wide">
<h2>📝 Recently Updated</h2>

<ul>
<li><a href="#">Thoughts on Seminar Supervision</a></li>
<li><a href="#">Image Analysis Practical Notes</a></li>
<li><a href="#">Single-Nucleus Sequencing</a></li>
</ul>

</div>

</div>
