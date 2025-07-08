---
layout: page
title: Posts
permalink: /posts/
---

# Alle Beiträge

Hier finden Sie alle Beiträge zur experimentellen Untersuchung "Denken oder Denken Lassen".

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

*{{ post.date | date: "%d.%m.%Y" }} von {{ post.author }}*

{% if post.excerpt %}
{{ post.excerpt | strip_html | truncatewords: 50 }}
{% else %}
{{ post.content | strip_html | truncatewords: 50 }}
{% endif %}

[Weiterlesen →]({{ post.url | relative_url }})

---

{% endfor %}

{% if site.posts.size == 0 %}
*Noch keine Beiträge vorhanden.*
{% endif %}
