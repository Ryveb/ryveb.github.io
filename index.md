---
layout: default
---

# My Security Blog

Offensive Security, Red Teaming and Research

## Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%d-%m-%Y" }}
{% endfor %}
