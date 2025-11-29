---
title: "Blog"
permalink: /blog/
---

## Articles

{% for post in paginator.posts %}
- <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a> — {{ post.date | date: "%b %-d, %Y" }}  
  {{ post.excerpt | strip_html | truncate: 140 }}
{% endfor %}

{% if paginator.total_pages > 1 %}
<div class="pagination">
  {% if paginator.previous_page %}
  <a href="{{ paginator.previous_page_path | relative_url }}">&laquo; Newer</a>
  {% endif %}
  {% if paginator.next_page %}
  <a href="{{ paginator.next_page_path | relative_url }}">Older &raquo;</a>
  {% endif %}
</div>
{% endif %}
