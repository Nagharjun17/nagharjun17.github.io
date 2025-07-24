---
layout: default
title: "Home"
---

# Hi, I'm **Nagharjun Mathi Mariappan** 👋

<img src="{{ 'assets/img/projects/passport-new.jpg' | relative_url }}"
     alt="Nagharjun Mathi Mariappan"
     class="headshot">

A **Data scientist** focused on turning raw biomedical data into reliable, actionable tools for clinicians. I design and ship end-to-end machine learning systems from data pipelines and model training to containerised, GPU backed deployments on Kubernetes with built-in tracking, CI/CD, and drift monitoring. Comfortable moving across the stack: **Python and PyTorch for modelling, MLflow for experiment management, GitHub Actions for automation, and FastAPI and LLMs for user-facing services**.

Adept at balancing research rigour with production constraints, I enjoy collaborating with physicians and engineers alike to bring models safely into everyday workflows. Constantly learning, open-sourcing when I can, and motivated by projects that improve patient care and scientific insight.

Beyond my professional work, I enjoy playing soccer.

---

## Latest Writing
{% for post in site.posts limit:3 %}
* **[{{ post.title }}]({{ post.url | relative_url }})** – {{ post.date | date:"%b %d, %Y" }}
{% endfor %}

[Explore all posts »]({{ '/blog/' | relative_url }})

---

## Selected Projects
{% assign feat = site.projects | sort:'year' | reverse | slice:0,3 %}
{% for p in feat %}
* **[{{ p.title }}]({{ p.url | relative_url }})** – {{ p.excerpt }}
{% endfor %}

[See all projects »]({{ '/projects/' | relative_url }})

---

## Education

| Degree                    | School              | Year | GPA     |
|---------------------------|---------------------|------|---------|
| MS Computer Engineering | New York University | 2024 | 3.96/4.0 |
| B.Tech Electronics and Computer Engineering | Vellore Institute of Technology | 2022 | 8.67/10 |



---

## Contact
- 📧 [nagharjun2000@gmail.com](mailto:nagharjun2000@gmail.com)
- 👔 [LinkedIn](https://www.linkedin.com/in/nagharjun-mathi-mariappan-b61499169/)
- 🧑‍💻 [GitHub](https://github.com/Nagharjun17)
- 📞 +1 (917) 688‑8843
