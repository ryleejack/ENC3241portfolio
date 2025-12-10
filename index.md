
---
layout: default
title: Home
---

# Portfolio

Select an assignment below and publish your work.

{% assign ordered = site.assignments | sort: 'due' %}
<ul class="assignments">
{% for a in ordered %}
  <li>
    <a href="{{ a.url }}">{{ a.title }}</a>
    <span class="due">Due: {{ a.due }} ({{ a.week }})</span>
  </li>
{% endfor %}
</ul>
