---
layout: default
title: Research
permalink: /research/
description: "Publications and working papers. Demo content for the Offprint theme."
---

My work is about the infrastructure of information distribution: how it is built, what it costs, and who it reaches.

## Publications

{% for item in site.data.publications %}{% unless item.status == 'wip' %}{% include publication.html pub=item %}{% endunless %}{% endfor %}

## Works in progress

{% for item in site.data.publications %}{% if item.status == 'wip' %}{% include publication.html pub=item %}{% endif %}{% endfor %}
