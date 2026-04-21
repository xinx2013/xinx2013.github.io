---
title: "XX-Lab - Team"
layout: gridlay
excerpt: "XX-Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

Jump to [staff](#staff), [students](#students).

<div markdown="0">

<h2 id="staff">Staff</h2>
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}<div class="row">{% endif %}
<div class="col-sm-6">
<div class="member-card{% if member.website %} clickable{% endif %}" {% if member.website %}onclick="window.location='{{ member.website }}'" style="cursor:pointer;"{% endif %}>
  <img src="{{ site.baseurl }}/photos/{{ member.photo }}" style="width:120px; height:120px; object-fit:cover; object-position:top; margin-right:15px; border-radius:4px;" />
  <div class="member-info">
    <h4 style="margin-top:0;">{{ member.name }}</h4>
    <i>{{ member.info }}</i>
    {% if member.description and member.description != "" %}
    <p style="margin-top:5px; font-size:13px; margin-bottom:0;">{{ member.description }}</p>
    {% endif %}
  </div>
</div>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}</div>{% endif %}
{% endfor %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}</div>{% endif %}

<h2 id="students">Students</h2>
{% assign number_printed = 0 %}
{% for member in site.data.students %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}<div class="row">{% endif %}
<div class="col-sm-6">
<div class="member-card{% if member.website %} clickable{% endif %}" {% if member.website %}onclick="window.location='{{ member.website }}'" style="cursor:pointer;"{% endif %}>
  <img src="{{ site.baseurl }}/photos/{{ member.photo }}" style="width:120px; height:120px; object-fit:cover; object-position:top; margin-right:15px; border-radius:4px;" />
  <div class="member-info">
    <h4 style="margin-top:0;">{{ member.name }}</h4>
    <i>{{ member.info }}</i>
    {% if member.description and member.description != "" %}
    <p style="margin-top:5px; font-size:13px; margin-bottom:0;">{{ member.description }}</p>
    {% endif %}
  </div>
</div>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}</div>{% endif %}
{% endfor %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}</div>{% endif %}

</div>
