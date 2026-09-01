---
layout: default
title: Research
permalink: /research/
description: Publications, policy reports, and work in progress by Daniel Kaufmann.
---

## Articles in journals

{% for p in site.data.publications.articles %}{% include publication.html item=p %}{% endfor %}

## Selected other publications

{% for p in site.data.publications.other %}{% include publication.html item=p %}{% endfor %}

## Work in progress

{% for p in site.data.publications.work_in_progress %}{% include publication.html item=p %}{% endfor %}
