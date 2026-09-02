---
layout: default
title: Data
permalink: /data/
description: Datasets constructed by Daniel Kaufmann, and links to data maintained by others.
---

<p class="pub-buttons section-nav">
  <a class="btn" href="#my-data">My data</a>
  <a class="btn" href="#other-data">Data by other researchers</a>
  <a class="btn" href="#historical-data">Historical</a>
  <a class="btn" href="#modern-data">Modern</a>
</p>

## My data {#my-data}

Here you can find data constructed in the course of my research projects.

{% for d in site.data.datasets %}{% include dataset.html item=d %}{% endfor %}

## Data by other researchers {#other-data}

I also assembled a variety of free data sources by other researchers and institutions that I found helpful in my research and policy work.

### Historical data {#historical-data}

{% for group in site.data.datalinks.historical %}
<h4>{{ group.region }}</h4>
{% include datatable.html items=group.items %}
{% endfor %}

### Modern data {#modern-data}

{% for group in site.data.datalinks.modern %}
<h4>{{ group.region }}</h4>
{% include datatable.html items=group.items %}
{% endfor %}
