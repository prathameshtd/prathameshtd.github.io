---
layout: page
permalink: /publications/
title: Research
description: Please stay tuned for the latest research!
years: []
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
