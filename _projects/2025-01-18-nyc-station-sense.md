---
layout: default
title: "NYC Station Sense"
year: 2024
stack: "Apache Spark • PySpark • SparkML • Python"
excerpt: "Parallel Spark pipeline that forecasts subway crowding with R² = 0.62."
tags: [Big Data, Time Series]
image: assets/img/projects/nyc-subway.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}


* **Parallelised** ETL on **11 M+** MTA entries/exits with Spark SQL & DataFrames.  
* **Engineered** temporal & weather features; trained SparkML regressors (GBT, RF).  
* Achieved **R² = 0.62** for 30‑minute ahead crowd prediction across all stations.  
* Enabled real‑time dashboards to surface hotspots for commuters.  

[GitHub Repo](https://github.com/Nagharjun17/Big_Data_Project/tree/main)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
