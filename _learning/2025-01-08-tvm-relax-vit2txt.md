---
layout: default
title: "TVM Relax: ViT→Text Mini Demo (RTX 3060)"
year: 2025
stack: "Python • TVM • CUDA"
excerpt: "Benchmarking a Vision Transformer encoder + transformer decoder in TVM Relax with baseline vs. optimized pipelines."
tags: [TVM, Relax, CUDA, Transformer, ViT]
image: assets/img/projects/tvm-relax-vit2txt.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}

YOU CAN REPLICATE THIS PROJECT -> https://github.com/Nagharjun17/Multimodal-Architecture-Optimisation-on-RTX3060-using-TVM

* Built a **Vision Transformer encoder + transformer decoder** pipeline in **TVM Relax** (not a trained model, random weights).
* Compiled two pipelines on RTX 3060 (float16):
  - **baseline_3060** → default legalization/fusion schedule
  - **opt_vit2txt** → optimized with dlight scheduling for matmuls & reductions
* Benchmarked encode + single-token decode:
  - Encode: 666.5 ms → 24.4 ms (**~96% faster**)
  - Decode: 744.5 ms → 22.6 ms (**~97% faster**, 1.3 tok/s → 44.2 tok/s)
* Demonstrated full flow: IRModule export → compilation → CUDA execution.

[GitHub Repo](https://github.com/Nagharjun17/Multimodal-Architecture-Optimisation-on-RTX3060-using-TVM)

<div style="margin-top: 2rem;">
  <a href="/learning" style="text-decoration: none; font-weight: bold;">← Back</a>
</div>
