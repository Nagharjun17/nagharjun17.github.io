---
layout: default
title: "Blog / Tutorials"
---

## Posts on This Site
{% if site.posts == empty %}
.......
{% else %}
{% for post in site.posts %}
* **[{{ post.title }}]({{ post.url | relative_url }})** – {{ post.date | date:"%b %d %Y" }}
  {% if post.tags %}<small>[{{ post.tags | join:", " }}]</small>{% endif %}
{% endfor %}
{% endif %}

---

## Elsewhere (Medium / TDS)
{% for ext in site.data.external_posts %}
* **[{{ ext.title }}]({{ ext.url }})** – {{ ext.date | date:"%b %d %Y" }} <small>({{ ext.source }})</small>
  {% if ext.tags %}<small>[{{ ext.tags | join:", " }}]</small>{% endif %}
{% endfor %}
