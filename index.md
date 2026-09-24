---
layout: default
title: "Security Blog"
---

# Welcome to my security blog

Offensive Security, Red Teaming, Research, Discussion pieces

## Posts

{% for post in site.posts %}

### [{{ post.title }}]({{ post.url | relative_url }})

*{{ post.date | date: "%d %B %Y" }}*

{% if post.description %}
{{ post.description }}
{% endif %}

---

{% endfor %}
