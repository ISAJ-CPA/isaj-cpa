---
layout: default
title: ホーム
---
<img width="1265" height="488" alt="NXVH2802" src="https://github.com/user-attachments/assets/0d4476b5-ccc6-4ec5-b95c-3cd8f17bfa13" />

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

## 免責事項
当サイトの内容は、作成時点における一般的な情報提供を目的としたものであり、特定の取引、会計処理、税務処理、法的判断その他の個別事案について助言を行うものではありません。また、当サイトに記載された見解は筆者個人のものであり、筆者に関連する法人、団体、組織等の見解を示すものではありません。制度改正や実務上の取扱いの変更等により、内容が最新でなくなる場合があります。実際の判断にあたっては、個別の状況に応じて専門家または関係機関にご確認ください。
