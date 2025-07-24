---
layout: default
title: "Skin Lesion Segment & Classify"
year: 2022
stack: "TensorFlow • React • Flask • Cloud Firestore"
excerpt: "Full‑stack web‑app that diagnoses 7 skin diseases at 89 % accuracy."
tags: [Healthcare, Web App, Deep Learning]
image: assets/img/projects/skin-cancer.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}


* Built a **two‑stage U‑Net ✚ CNN** pipeline—segmentation + classification.  
* Achieved **89.3 % accuracy / 89.1 % precision** over 7 lesion classes (HAM10000).  
* Deployed interactive React front‑end + Flask API; state saved in Firestore.  
* Designed for dermatologists to expedite early‑stage cancer screening.  

[GitHub Repo](https://github.com/Nagharjun17/Skin-Cancer-Detection-User-Interface?tab=readme-ov-file)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
