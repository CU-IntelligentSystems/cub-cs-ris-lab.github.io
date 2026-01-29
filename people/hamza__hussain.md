---
title: "Hamza Hussain"
layout: default
parent: People
nav_order: 2

name: Hamza
last_name: Hussain
group: masters

honorific_title:
last_degree: Bachelors
public_url:
status: active
offboard: no
research_focus:
projects: [acoustic-modem-energy-management]
---

# {{ page.name }} {{ page.last_name }}
{: .no_toc }

{{ page.research_focus }}
{: .fs-6 .fw-300 }

---

## About

*Coming soon...*

## Current Projects

{% for project_slug in page.projects %}
- [{{ project_slug }}]({{ '/projects/' | append: project_slug | append: '/' | relative_url }})
{% endfor %}

## Related WIP Entries

{% assign person_wips = site.pages | where_exp: "p", "p.path contains 'wip/'" | where_exp: "p", "p.presenter == page.name or p.presenter contains page.name" | sort: "date" | reverse %}
{% if person_wips.size > 0 %}
{% for wip in person_wips %}
- [{{ wip.title }}]({{ wip.url | relative_url }}) - {{ wip.date | date: "%Y-%m-%d" }}
{% endfor %}
{% else %}
*No WIP entries yet.*
{% endif %}
