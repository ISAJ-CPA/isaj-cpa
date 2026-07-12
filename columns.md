---
layout: page
title: コラム一覧
---
{% for post in site.posts %}
- {{ post.date | date: "%Y-%m-%d" }}：[{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
