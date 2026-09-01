---
layout: default
title: Research
permalink: /research/
description: Published articles and working papers by Daniel Kaufmann.
---

{: .note }
*All entries below are placeholders. The real list is ported in Phase 2 —
editing `_data/publications.yml` is all that is needed.*

## Articles in journals

{% for p in site.data.publications.articles %}{% include publication.html item=p %}{% endfor %}

## Working papers

{% for p in site.data.publications.working_papers %}{% include publication.html item=p %}{% endfor %}
