---
layout: page
title: Latest
permalink: /latest/
---

{% assign page_start = 2 %}
{% assign page_end = paginator.total_pages %}

{% for index in (page_start..page_end) %}
  {{ site.paginate_path | replace: ':num', index | relative_url }}
{% endfor %}
