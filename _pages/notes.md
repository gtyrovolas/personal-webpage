---
layout: page
permalink: /notes/
title: notes
description: Notes for courses I took.
years: [2020, 2022]
nav: true
---

<div class="publications">
    {% for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {% bibliography -f papers -q @*[year={{y}}]* %}
    {% endfor %}
</div>