---
layout: default
title: "Image Captioning using ViT"
year: 2024
stack: "Vision Transformer • Transformer Decoder • PyTorch • Flickr8K"
excerpt: "ViT + decoder model that scores BLEU‑4 19.6 on Flickr8K."
tags: [NLP, Vision, Transformers]
image: assets/img/projects/image-caption.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}


* **Extracted** image embeddings with a pre‑trained Vision Transformer encoder.  
* **Trained** a Transformer decoder on GloVe token embeddings to generate captions.  
* Reached **BLEU‑4 = 19.6**—competitive with CNN‑based baselines.  
* Out‑of‑the‑box inference wrapper enables accessibility alt‑text generation.  

[GitHub Repo](https://github.com/Nagharjun17/ImageCaptioningUsingVisionTransformer/tree/main?tab=readme-ov-file)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
