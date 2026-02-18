---
layout: page
title: about
permalink: /about/
---

<img src="/assets/img/marcelo.png"
     alt="Profile photo"
     style="width: 180px; float: right; margin: 0 0 1em 1em; border-radius: 6px;">

I am an Associate Professor at Federal University of Pampa in Brazil where I lead the LOS Research Lab.

My research interests cover a broad spectrum of topics in both networks, systems, and optimization. More specifically, Software-Defined Networking, Network Function Virtualization, and Programmable Data Planes. Details of my publications can be found on my Google Scholar profile or my publications page.

I am always looking for motivated students. If you have interests similar to mine, feel free to reach out!

News

{% assign items = site.news | sort: "date" | reverse %}
{% for item in items limit:5 %}
- **{{ item.date | date: "%b %d, %Y" }}** — [{{ item.title }}]({{ item.url }})
{% endfor %}
