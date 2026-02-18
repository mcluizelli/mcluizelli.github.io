---
layout: page
title: news
permalink: /news/
---

{% assign items = site.news | sort: "date" | reverse %}
{% for item in items %}
**{{ item.date | date: "%b %d, %Y" }} — {{ item.title }}**  
{{ item.content | markdownify }}

{% endfor %}
