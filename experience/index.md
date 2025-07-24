---
layout: default
title: "Experience"
---

{% assign jobs = site.experience | sort:'start' | reverse %}
{% for job in jobs %}
## {{ job.title }} – {{ job.company }}
{{ job.start | date:"%b %Y" }} – {{ job.end | date:"%b %Y" }} • {{ job.location }}

{{ job.content | markdownify }}

---
{% endfor %}
