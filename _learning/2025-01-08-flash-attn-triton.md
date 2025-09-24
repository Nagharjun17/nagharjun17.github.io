---
layout: default
title: "Flash Attention in Triton"
year: 2025
stack: "Python • PyTorch • Triton"
excerpt: "Custom implementation of Flash Attention forward/backward kernels with benchmarking."
tags: [Triton, PyTorch, FlashAttention, GPU]
image: assets/img/projects/flash-attn-triton.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}

YOU CAN REPLICATE THIS PROJECT -> https://github.com/Nagharjun17/Flash-Attention-Triton

* Implemented custom **Flash Attention** forward & backward kernels in Triton with causal mask support.
* Integrated with PyTorch using `autograd.Function` for seamless gradient computation.
* Benchmarked kernels vs. plain PyTorch math baseline → **~2.5× speedup** (f+b runtime: 2.757 ms → 1.116 ms on RTX GPU).
* Added handwritten notes (PDF) with forward/backward derivations for better theoretical grounding.
* Tested with PyTorch 2.3 + Triton 2.1 on RTX hardware.

[GitHub Repo](https://github.com/Nagharjun17/Flash-Attention-Triton)

<div style="margin-top: 2rem;">
  <a href="/learning" style="text-decoration: none; font-weight: bold;">← Back</a>
</div>
