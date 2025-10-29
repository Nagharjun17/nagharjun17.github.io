---
layout: default
title: "Wi-Fi Extender LED Fault Detection on Kria KV260"
year: 2025
stack: "Python • Vitis AI • Kria KV260"
excerpt: "Detect power loss by watching the extender’s LED and send instant alerts."
tags: [Edge AI, Fault Detection]
image: assets/img/projects/fdet.png
---

{% if page.image %}

<figure> <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy" width="540" style="height:auto;"> <figcaption>{{ page.title }}</figcaption> </figure> {% endif %}

**YOU CAN REPLICATE THIS PROJECT -> https://github.com/Nagharjun17/KV260-LED-Fault-Detector**

* Used a 13MP AR1335 IAS camera with a fixed ROI over the LED to classify on vs off.
* Trained a tiny CNN on 96x96 crops and compiled to INT8 with Vitis AI for the DPU.
* Ran real time inference on the KV260 with simple temporal filtering to avoid flicker.
* Published state and alerts via MQTT.

**[GitHub Repo](https://github.com/Nagharjun17/KV260-LED-Fault-Detector)**

<div style="margin-top: 2rem;"> <a href="/learning" style="text-decoration: none; font-weight: bold;">← Back</a> </div>