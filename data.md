---
layout: default
title: Data
permalink: /data/
description: Datasets constructed by Daniel Kaufmann, and links to data maintained by others.
---

<p class="pub-buttons section-nav">
  <a class="btn" href="#my-data">My data</a>
  <a class="btn" href="#other-data">Data by other researchers</a>
</p>

## My data {#my-data}

Datasets constructed in the course of various research projects.

{% for d in site.data.datasets %}{% include dataset.html item=d %}{% endfor %}

## Data by other researchers {#other-data}

### Historical data

{% for group in site.data.datalinks.historical %}
<h4>{{ group.region }}</h4>
<ul class="linklist">
{%- for i in group.items %}
  <li><span class="linkname">{{ i.name }}</span> — {{ i.description }}
    {%- for l in i.links %} <a href="{{ l.url }}">{{ l.label }}</a>{% unless forloop.last %} ·{% endunless %}{% endfor %}</li>
{%- endfor %}
</ul>
{% endfor %}

### Modern data

{% for group in site.data.datalinks.modern %}
<h4>{{ group.region }}</h4>
<ul class="linklist">
{%- for i in group.items %}
  <li><span class="linkname">{{ i.name }}</span> — {{ i.description }}
    {%- for l in i.links %} <a href="{{ l.url }}">{{ l.label }}</a>{% unless forloop.last %} ·{% endunless %}{% endfor %}</li>
{%- endfor %}
</ul>
{% endfor %}
