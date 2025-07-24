---
layout: default
title: "Fine‑Tuning GPT‑3"
year: 2022
stack: "GPT‑3 • OpenAI API • Weights & Biases • Python"
excerpt: "Few‑shot tuning pipeline that slashes prompt tokens > 60 %."
tags: [LLM, NLP]
image: assets/img/projects/gpt-tune.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}


* **Fine‑tuned** GPT‑3 (Davinci) for screenplay generation via transfer learning.  
* Searched hyper‑params (batch, lr, epochs) on W&B sweeps to optimise cost ↔ quality.  
* Cut prompt token count **> 60 %** while preserving narrative structure.  
* Published a guide to economical GPT‑3 tuning for resource‑constrained teams.  

[GitHub Repo](https://github.com/Nagharjun17/Fine-Tuning-GPTs)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
