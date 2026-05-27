---
layout: default
title: Home
---

{% assign c = site.conference %}

{% if c.state == "inactive" %}

# Minnesota Workshop in Macroeconomic Theory

<p>The Minnesota Workshop in Macroeconomic Theory is a workshop on dynamic macroeconomic theory sponsored by the University of Minnesota and the Federal Reserve Bank of Minneapolis. It is held on the campus of the University of Minnesota.</p>

<p>Past programs are <a href="{{ '/past/' | relative_url }}">here</a>.</p>

<p>We welcome papers in a variety of areas. Examples of topics of interest include:</p>

{% include topics.html %}

<p>Papers in other areas are welcome as well. The final topics will be determined in large part by the interests of the participants.</p>

<p>The {{ c.year }} conference will last for three days in the {{ c.dates_general }}. The schedule will include roughly {{ c.num_talks }} talks. There will also be ample time for informal discussions among the participants.</p>

<p>The call for papers will be announced on this page.</p>

<p>Details on the program, travel, hotel, and other administrative details will be posted on this website as we get closer to the date of the conference.</p>

{% elsif c.state == "cfp" %}

# Minnesota Macro {{ c.year }}

<p>The Minnesota Workshop in Macroeconomic Theory is a workshop on dynamic macroeconomic theory sponsored by the University of Minnesota and the Federal Reserve Bank of Minneapolis. It is held on the campus of the University of Minnesota.</p>

<p>The {{ c.year }} conference will last for three days, from {{ c.dates_long }}.</p>

<p class="callout">If you are interested in presenting, please submit your paper by <strong>{{ c.submission_deadline }}</strong> using this form: <a href="{{ c.submission_url }}">{{ c.submission_url }}</a></p>

<p>Details on the program, travel, hotel, and other administrative details will be posted on this website as we get closer to the date of the conference.</p>

<hr>

<p>The schedule will include roughly {{ c.num_talks }} talks. There will also be ample time for informal discussions among the participants. We request that all participants attend the entire three days of the conference.</p>

<p>We welcome papers in a variety of areas. Examples of topics of interest include:</p>

{% include topics.html %}

<p>Papers in other areas are welcome as well. The final topics will be determined in large part by the interests of the participants.</p>

<p>Please feel free to pass news of this conference on to other potentially interested people.</p>

{% elsif c.state == "deadline_passed" %}

# Minnesota Macro {{ c.year }}

<p>The Minnesota Workshop in Macroeconomic Theory is a workshop on dynamic macroeconomic theory sponsored by the University of Minnesota and the Federal Reserve Bank of Minneapolis. It is held on the campus of the University of Minnesota.</p>

<p>The {{ c.year }} conference will last for three days, from {{ c.dates_long }}.</p>

<p class="callout">The submission deadline has passed.</p>

<p>Details on the program, travel, hotel, and other administrative details will be posted on this website as we get closer to the date of the conference.</p>

<hr>

<p>The schedule will include roughly {{ c.num_talks }} talks. There will also be ample time for informal discussions among the participants. We request that all participants attend the entire three days of the conference.</p>

{% elsif c.state == "active" %}

# Minnesota Macro {{ c.year }}

<p>The Minnesota Workshop in Macroeconomic Theory is a workshop on dynamic macroeconomic theory sponsored by the University of Minnesota and the Federal Reserve Bank of Minneapolis. It is held on the campus of the University of Minnesota.</p>

<p>The {{ c.year }} conference will last for three days, from {{ c.dates_long }}.</p>

<p class="callout"><a href="{{ '/program/' | relative_url }}"><strong>Minnesota Macro {{ c.year }} Program</strong></a></p>

<p>The conference will take place on the {{ c.venue_html }}.</p>

<p>We expect all participants to attend the three days of the conference. If you plan to attend, please <a href="{{ '/registration/' | relative_url }}">register before {{ c.registration_deadline }}</a>.</p>

<p><a href="{{ '/hotel/' | relative_url }}">Reserve your room before {{ c.hotel_deadline }}</a>.</p>

{% endif %}

## {{ site.conference.year }} Program Organizers

<ul class="organizer-list">
  <li><strong>Alessandra Fogli</strong> — Federal Reserve Bank of Minneapolis</li>
  <li><strong>Pablo Kurlat</strong> — University of Southern California</li>
</ul>

## Permanent Organizers

<ul class="organizer-list">
  <li><strong>Manuel Amador</strong> — Federal Reserve Bank of Minneapolis and University of Minnesota</li>
  <li><strong>Cristina Arellano</strong> — Federal Reserve Bank of Minneapolis</li>
</ul>
