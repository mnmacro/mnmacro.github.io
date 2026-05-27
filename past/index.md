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
    {% if p.organizers %}
      {%- assign organizer_names = "" -%}
      {%- assign chunks = p.organizers | append: "|END|" | split: "(" -%}
      {%- for chunk in chunks -%}
        {%- if forloop.first -%}
          {%- assign organizer_names = chunk -%}
        {%- else -%}
          {%- assign after = chunk | split: ")" | last -%}
          {%- assign organizer_names = organizer_names | append: after -%}
        {%- endif -%}
      {%- endfor -%}
      {%- assign organizer_names = organizer_names | replace: "|END|", "" | replace: "  ", " " | strip -%}
      <p class="organizers">{{ organizer_names }}</p>
    {% endif %}
  </a>
{% endfor %}
</div>
