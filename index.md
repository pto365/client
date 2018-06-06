---
title: Pages
---

| Title | Link | Language |
| --- | --- |{% assign allPages = site.pages | sort: 'url' %}
{% for page in  allPages %}| {{page.title}} | <a href="{{site.baseurl}}{{ page.url }}"> ({{ page.url }})</a> | {{ page.language }} |
{% endfor %}
