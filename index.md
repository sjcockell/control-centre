---
layout: default
title: Dashboard
nav_order: 1
---

# Dashboard

<div class="dashboard-grid">

<div class="dashboard-card">
<h2>🎓 Teaching</h2>

{% for item in site.data.bookmarks.teaching %}
[<i class="fa-solid {{ item.icon }}"></i> {{item.name}}]({{item.url}}){: .btn }
{% endfor %}

</div>

<div class="dashboard-card">
<h2>🧬 Research</h2>

<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov">PubMed</a></li>
<li><a href="/research/">tes</a></li>
</ul>

</div>

<div class="dashboard-card">
<h2>📓 Journal</h2>

<ul>
<li><a href="/journal/">Recent Entries</a></li>
<li><a href="projects/">Project Log</a></li>
</ul>

</div>

<div class="dashboard-card">
<h2>✅ Tasks</h2>

<ul>
<li><a href="https://github.com/users/YOURUSERNAME/projects/1">Teaching</a></li>
<li><a href="https://github.com/users/YOURUSERNAME/projects/2">Research Board</a></li>
<li><a href="https://github.com/users/YOURUSERNAME/projects/3">Personal</a></li>
</ul>

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
