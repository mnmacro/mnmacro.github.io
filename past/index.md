---
layout: default
title: Past Conferences
permalink: /past/
---

# Past Conferences

<ul class="past-index">
{% for year in site.past_years %}
  <li><a href="{{ '/past/' | append: year | append: '/' | relative_url }}">MN Macro {{ year }}</a></li>
{% endfor %}
</ul>
