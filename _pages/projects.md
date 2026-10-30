---
layout: page
title: projects
permalink: /projects/
description: Open-source platforms and systems projects.
nav: true
nav_order: 3
---

{% assign projects = site.projects | sort: 'importance' %}
{% for project in projects %}

## [{{ project.title }}]({{ project.url | relative_url }})

{{ project.description }}

{% endfor %}
