---
layout: default
title: "Interactive Multiple Regression"
year: 2023
stack: "scikit‑learn • Pandas • Matplotlib • ipywidgets"
excerpt: "Notebook widget that visualises how features shift insurance pricing."
tags: [Data Viz, Regression]
image: assets/img/projects/interactive-regression.gif
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}


* **Built** a linear‑regression model on U.S. medical‑cost data.  
* Selected predictors via correlation matrix + ANOVA significance tests.  
* Achieved **$4 256 MAE** on hold‑out set.  
* Added ipywidgets sliders so users can tweak BMI, age, smokers‑flag in real time.  

[GitHub Repo](https://github.com/Nagharjun17/Interactive-Linear-Regression-using-Widgets)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
