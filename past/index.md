---
layout: default
title: Past Conferences
permalink: /past/
---

# Past Conferences

<div class="past-cards">
{% for year in site.past_years %}
  {% assign permalink = '/past/' | append: year | append: '/' %}
  {% assign p = site.pages | where: "permalink", permalink | first %}
  <a class="past-card" href="{{ permalink | relative_url }}">
    <h2>MN Macro {{ year }}</h2>
    {% if p.dates %}<p class="dates">{{ p.dates }}</p>{% endif %}
    {% if p.organizers %}<p class="organizers">{{ p.organizers }}</p>{% endif %}
  </a>
{% endfor %}
</div>
