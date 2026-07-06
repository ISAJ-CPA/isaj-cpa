---
layout: default
title: ホーム
---

## 新着コラム

{% if site.posts.size > 0 %}
<ul class="post-list">
  {% for post in site.posts limit:5 %}
  <li>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>：<a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>

<p><a href="{{ '/columns.html' | relative_url }}">コラム一覧を見る</a></p>
{% else %}
<p>今後、会計・監査に関するコラムを追加していきます。</p>
<p>鋭意製作中です。</p>
{% endif %}
