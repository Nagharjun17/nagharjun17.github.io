---
layout: default
title: "Wi-Fi Extender LED Fault Detection on Kria KV260"
year: 2025
stack: "Python • PyTorch • ONNX Runtime • Kria KV260"
excerpt: "Detect Wi-Fi extender power loss by watching its status LED and sending instant alerts."
tags: [Edge AI, Fault Detection]
image: assets/img/projects/fdet.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot"
     loading="lazy" width="540" style="height:auto;">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}

**YOU CAN REPLICATE THIS PROJECT -> https://github.com/Nagharjun17/Fault-Detection---WiFi-Extender**

* Used a 13 MP AR1335 camera pointed at the Wi-Fi extender LED to detect power loss.
* Trained a MobileNetV2 classifier on LED on vs off images using PyTorch and timm on my laptop.
* Exported the best model to ONNX and ran real time inference on the Kria KV260 using ONNX Runtime and the SmartCam RTSP stream.
* Added simple temporal filtering and thresholds so short flickers do not trigger false alarms.
* Published LED state and class probabilities to MQTT topics (via HiveMQ Cloud) so any service can subscribe and alert.

**[GitHub Repo](https://github.com/Nagharjun17/Fault-Detection---WiFi-Extender)**  
**[Demo Video](https://youtube.com/shorts/JjFDnCMGacQ)**

<div style="margin-top: 2rem;">
  <a href="/learning" style="text-decoration: none; font-weight: bold;">← Back</a>
</div>
