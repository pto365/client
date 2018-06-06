---
title: Sitemap
layout: page
---
<ul>
{% assign allPages = site.pages | sort: 'url' %}
 {% for page in  allPages %}
<li >
    <a href="{{site.baseurl}}{{ page.url }}">{{page.title}} ({{ page.url }})</a>
</li>
            
{% endfor %}
</ul>
