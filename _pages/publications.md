---
title: "XX-Lab - Publications"
layout: gridlay
excerpt: "XX-Lab -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors | replace: "Xin Xin", "<span style='color:#2196F3; font-weight:normal;'>Xin Xin</span>" | replace: "Fan Li", "<strong>Fan Li</strong>" | replace: "Ruizhi Zhu", "<strong>Ruizhi Zhu</strong>" }} </em><br />{{ publi.link.display }}{% if publi.paper %} [<a href="{{ publi.paper }}">paper</a>]{% endif %}{% if publi.slide %} [<a href="{{ publi.slide }}">slide</a>]{% endif %}

{% endfor %}
