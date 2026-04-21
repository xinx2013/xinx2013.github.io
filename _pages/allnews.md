---
title: "News"
layout: textlay
excerpt: "Xin's Lab - News"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br> {{ article.headline }}</p>
{% endfor %}
