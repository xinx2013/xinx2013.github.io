---
title: "MemArch-Lab - Publications"
layout: gridlay
excerpt: "MemArch-Lab -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

<div id="selected-pub-list">

## Selected Publications

{% for publi in site.data.publist %}
{% if publi.selected == 1 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors | replace: "Xin Xin", "<span style='color:#2196F3; font-weight:normal;'>Xin Xin</span>" | replace: "Fan Li", "<strong>Fan Li</strong>" | replace: "Ruizhi Zhu", "<strong>Ruizhi Zhu</strong>" }} </em><br />{{ publi.link.display }}{% if publi.paper %} [<a href="{{ publi.paper }}">paper</a>]{% endif %}{% if publi.slide %} [<a href="{{ publi.slide }}">slide</a>]{% endif %}

{% endif %}
{% endfor %}

</div>

<p id="see-full-link"><a href="javascript:void(0);" onclick="document.getElementById('full-pub-list').style.display='block'; document.getElementById('selected-pub-list').style.display='none'; document.getElementById('see-full-link').style.display='none';" style="font-weight:bold;">>> See full list of publications</a></p>

<div id="full-pub-list" style="display:none;">

## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors | replace: "Xin Xin", "<span style='color:#2196F3; font-weight:normal;'>Xin Xin</span>" | replace: "Fan Li", "<strong>Fan Li</strong>" | replace: "Ruizhi Zhu", "<strong>Ruizhi Zhu</strong>" }} </em><br />{{ publi.link.display }}{% if publi.paper %} [<a href="{{ publi.paper }}">paper</a>]{% endif %}{% if publi.slide %} [<a href="{{ publi.slide }}">slide</a>]{% endif %}

{% endfor %}

</div>
