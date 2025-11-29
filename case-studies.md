---
title: "Case Studies & Testimonials"
permalink: /case-studies/
---

## Case studies

Real examples of applied work. Details are anonymized where required.

{% for cs in site.case_studies %}
- <a href="{{ cs.url | relative_url }}"><strong>{{ cs.title }}</strong></a><br>
  {{ cs.summary }}
{% endfor %}

## Testimonials

> "Placeholder testimonial from a coach or athlete about clarity, structure, and impact."

Add real testimonials as you collect them.
