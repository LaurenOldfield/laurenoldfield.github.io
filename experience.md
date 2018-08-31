---
layout: default
title: Professional Experience | Alexander Titus
description: The professional experience from Titus Analytics
sitemap:
    priority: 0.7
    lastmod: 2017-1-28
    changefreq: weekly
---

<div class="container row">
    {% assign steps = site.steps | sort: 'date' | reverse %}
    {% for step in steps %}
    <div class="item">
        <!--<i class="vertical-line"></i>-->
        <h2 class="item-date">{{ step.date | date: '%m/%Y' }}{% if step.enddate %} - {{ step.enddate | date: '%m/%Y' }}{% endif %}</h2>
        <div class="card-panel">
            <h3 class="card-title">
                {{ step.title }}
            </h3>
            <p>
                {{ step.content }}
            </p>
        </div>
    </div>
    {% endfor %}
    
</div>
