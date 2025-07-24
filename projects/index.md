---
layout: default
title: "Projects"
---
<h2>Projects</h2>
<div class="projects-grid">
{% assign proj = site.projects | sort:'year' | reverse %}
{% for p in proj %}
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

## Research & Publications
* **A two‑stage atrous residual CNN for skin disease detection** – *Concurrency & Computation: Practice and Experience*.<br>
  <https://doi.org/10.1002/cpe.7834>
* **Gaussian‑dropout ensemble CNN for breast‑tumour ultrasound images** – *IRBM* 43(6).<br>
  <https://doi.org/10.1016/j.irbm.2022.02.006>
* **Disease detection in rice leaves using transfer learning** – *Journal of Physics: Conference Series* 1911(1).<br>
  <https://doi.org/10.1088/1742-6596/1911/1/012004>