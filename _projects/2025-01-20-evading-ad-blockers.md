---
layout: default
title: "Evading Ad‑Blockers"
year: 2024
stack: "YOLOv5 • PyTorch • OpenCV • Python"
excerpt: "Poisoned object‑detection model that drops ad‑blocking recall 15 %."
tags: [Computer Vision, AdTech]
image: assets/img/projects/adevade.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}


* **Trained** a YOLOv5 detector to recognise ads with **90 % mIoU** baseline accuracy.  
* **Crafted** adversarial image patches that reduce detection rates **15 %** while remaining visually innocuous.  
* **Analysed** specific convolutional filters to pinpoint vulnerability surfaces.  
* **Retrained & fine‑tuned** the model to assess recovery strategies.  

[GitHub Repo](https://github.com/Nagharjun17/Perceptual_Ad-Blocker_Evasion)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
