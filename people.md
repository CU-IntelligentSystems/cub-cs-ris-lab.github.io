---
title: People
layout: default
---

# People

This page lists all lab members and links to their WIP entries.

## Faculty

*Coming soon...*

## Graduate Students

*Coming soon...*

## Undergraduate Students

*Coming soon...*

---

## WIP Entries by Person

{% assign wip_posts = site.pages | where_exp: "page", "page.path contains 'wip/'" | where_exp: "page", "page.title contains 'WIP:'" %}
{% assign presenters = wip_posts | map: "presenter" | uniq | sort %}

{% if presenters.size > 0 %}
{% for presenter in presenters %}
### {{ presenter }}
{% assign presenter_posts = wip_posts | where: "presenter", presenter | sort: "date" | reverse %}
{% for post in presenter_posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y-%m-%d" }} - {{ post.project }}
{% endfor %}
{% endfor %}
{% else %}
*No WIP entries yet.*
{% endif %}
