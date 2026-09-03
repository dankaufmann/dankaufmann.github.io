---
layout: default
title: Research
permalink: /research/
description: Publications, policy reports, and work in progress by Daniel Kaufmann.
---

<p class="pub-buttons section-nav">
  <a class="btn" href="#articles-in-journals">Articles in journals</a>
  <a class="btn" href="#work-in-progress">Work in progress</a>
  <a class="btn" href="#selected-other-publications">Other publications</a>
</p>

## Articles in academic journals {#articles-in-journals}

{% for p in site.data.publications.articles %}{% include publication.html item=p %}{% endfor %}

## Work in progress {#work-in-progress}

{% for p in site.data.publications.work_in_progress %}{% include publication.html item=p %}{% endfor %}

## Other publications {#selected-other-publications}

{% for p in site.data.publications.other %}{% include publication.html item=p %}{% endfor %}
