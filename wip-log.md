---
title: WIP Log
layout: default
---

# Work-in-Progress Log

This page shows the latest WIP entries across all projects, newest first.

{% assign wip_posts = site.pages | where_exp: "page", "page.path contains 'wip/'" | where_exp: "page", "page.title contains 'WIP:'" | sort: "date" | reverse %}

{% if wip_posts.size > 0 %}
{% for post in wip_posts %}
## [{{ post.title }}]({{ post.url }})
**Date:** {{ post.date | date: "%Y-%m-%d" }}
**Project:** [{{ post.project }}](/projects/{{ post.project }}/)
**Presenter:** {{ post.presenter }}
**Status:** {{ post.status }}

---
{% endfor %}
{% else %}
*No WIP entries yet. Check back soon!*
{% endif %}
