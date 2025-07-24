---
layout: default
title: "NYC Citibike Dashboard"
year: 2024
stack: "AWS S3 • Snowflake • Airflow • Tableau"
excerpt: "Real‑time Citi Bike analytics powered by Snowpipe & Tableau Cloud."
tags: [Data Engineering, Tableau]
image: assets/img/projects/nyc-citibike.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}


* **Fetched** live Citi Bike feeds to S3; auto‑landed into Snowflake via Snowpipe.  
* Orchestrated hourly ETL with Airflow on EC2.  
* Published interactive availability dashboards in Tableau Cloud.  
* Used by city commuters to find docks in real‑time.  

[Live Demo](https://nagharjun17.github.io/nyc-citibike-analytics/) •  
[GitHub Repo](https://github.com/Nagharjun17/NYCitibike-Analytics)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
