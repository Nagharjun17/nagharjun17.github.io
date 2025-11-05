---
layout: default
title: "Home"
---

# Hi, I'm **Nagharjun Mathi Mariappan** 👋

<img src="{{ 'assets/img/projects/passport-new.jpg' | relative_url }}"
     alt="Nagharjun Mathi Mariappan"
     class="headshot">

**Data Scientist** focused on turning raw biomedical data into usable tools for clinicians. I design and deploy end to end machine learning systems from data pipelines and model training to containerised deployments on Docker on local and cloud based servers. Comfortable moving across the stack: **Python and PyTorch for modelling, MLflow for experiment tracking, GitHub Actions for automation, and FastAPI for services**.

Lately I have been exploring GPU programming, ML compilers, and model optimizations on hardware. I am experimenting with CUDA kernels, Triton, Apache TVM, MLIR/LLVM passes and containerised deployments.

<img src="{{ 'assets/img/projects/set.JPG' | relative_url }}"
     alt="Server"
     width="200"
     style="float:right; margin-left:15px; max-width:200px; height:auto;">

I enjoy collaborating with physicians and engineers to bring models into everyday workflows under various settings. Constantly learning, open sourcing when I can and motivated by interesting projects.

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
