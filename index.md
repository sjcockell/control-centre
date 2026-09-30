---
layout: default
title: Dashboard
nav_order: 1
---

# Dashboard

<div class="dashboard-grid">

<div class="dashboard-card">
<h2><i class="fa-solid fa-graduation-cap"></i> Teaching</h2>
{% for item in site.data.bookmarks.teaching %}
<a href="{{ item.url }}" class="btn"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}
</div>

<div class="dashboard-card">
<h2><i class="fa fa-empire"></i> Canvas</h2>
{% for item in site.data.bookmarks.modules %}
<a href="{{ item.url }}" class="btn"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}
</div>

<div class="dashboard-card">
<h2><i class="fa-solid fa-institution"></i> University Services</h2>
{% for item in site.data.bookmarks.university %}
<a href="{{ item.url }}" class="btn"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}
</div>

<div class="dashboard-card">
<h2><i class="fa-solid fa-microscope"></i> Research</h2>

<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov">PubMed</a></li>
<li><a href="/research/">tes</a></li>
</ul>

</div>

<div class="dashboard-card">
<h2><i class="fa-solid fa-book"></i> Journal</h2>

<ul>
<li><a href="/journal/">Recent Entries</a></li>
<li><a href="projects/">Project Log</a></li>
</ul>

</div>

<div class="dashboard-card">
<h2><i class="fa fa-check-square-o" aria-hidden="true"></i> Tasks</h2>


{% for item in site.data.bookmarks.tasks %}
<a href="{{ item.url }}" class="btn"><i class="{{ item.icon }}"></i> {{ item.name }}</a>
{% endfor %}


</div>

<div class="dashboard-card dashboard-wide">
<h2>🚀 Current Projects</h2>

<ul>
<li>First-Year Seminar Development</li>
<li>Bioinformatics Practical Redesign</li>
<li>Single-cell Teaching Resources</li>
</ul>

</div>

<div class="dashboard-card dashboard-wide">
<h2>📝 Recently Updated</h2>

<ul>
<li><a href="#">Thoughts on Seminar Supervision</a></li>
<li><a href="#">Image Analysis Practical Notes</a></li>
<li><a href="#">Single-Nucleus Sequencing</a></li>
</ul>

</div>

</div>
