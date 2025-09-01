---
layout: default
title: "Learning"
---
<h2>Learning new stuff</h2>
<div class="projects-grid">
{% assign learning = site.learning | sort:'year' | reverse %}
{% for p in learning %}
<article class="project-card">
  {% if p.image %}
    <a href="{{ p.url | relative_url }}">
      <img src="{{ p.image | relative_url }}" alt="{{ p.title }} screenshot" loading="lazy">
    </a>
  {% endif %}
  <div class="project-body">
    <h3>
      <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
      <span class="project-year">({{ p.year }})</span>
    </h3>
    <p class="project-stack">{{ p.stack }}</p>
    <p>{{ p.excerpt }}</p>
    <p><a href="{{ p.url | relative_url }}">Details →</a></p>
  </div>
</article>
{% endfor %}
</div>
