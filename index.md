---
layout: default
title: ホーム
---

![Top](assets/top.JPG)

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

## お役立ちリンク集
### 会計関連
- [ASBJ-会計基準検索システム](https://www.asb-j.jp/jp/accounting_standards_system.html)
- [IFRS-IFRS Foundation](https://www.ifrs.org/) 

### 開示関連
- [経団連-会社法施行規則及び会社計算規則による株式会社の各種書類のひな型](https://www.keidanren.or.jp/policy/hinagata.html)
- [FASF-有価証券報告書の作成要領等](https://www.fasf-j.jp/jp/disclosure.html)
- [SSBJ-サステナビリティ開示基準検索システム](https://www.ssb-j.jp/jp/ssbj_standards_system.html)
- [JPX-決算短信作成要領・四半期決算短信作成要領](https://www.jpx.co.jp/equities/listed-co/format/summary/index.html)

### 監査関連
- [JICPA-実務指針等公表物一覧](https://jicpa.or.jp/specialized_field/publication/)

### 東証関連
- [JPX-上場会社の決定・発生事実の開示様式例](https://www.jpx.co.jp/equities/listed-co/format/tddoc/index.html)
- [JPX-会社情報適時開示ガイドブック](https://www.jpx.co.jp/equities/listing/disclosure/guidebook/index.html)
- [JPX-不適正意見・意見不表明・限定付適正意見等一覧](https://www.jpx.co.jp/listing/others/adverse-opinion/index.html)
- [JPX-期中レビューの義務付け要件該当会社一覧](https://www.jpx.co.jp/listing/others/review/index.html)
- [JPX-有報等提出期限延長会社一覧](https://www.jpx.co.jp/listing/others/extended/index.html)
- [JPX-商号変更会社一覧](https://www.jpx.co.jp/listing/others/changed/index.html)

### その他
- [MURC-外国為替相場情報](https://www.murc-kawasesouba.jp/fx/index.php)
- [財務省-国債金利情報](https://www.mof.go.jp/jgbs/reference/interest_rate/index.htm)

## 免責事項
当サイトの内容は、作成時点における一般的な情報提供を目的としたものであり、特定の取引、会計処理、税務処理、法的判断その他の個別事案について助言を行うものではありません。また、当サイトに記載された見解は筆者個人のものであり、筆者に関連する法人、団体、組織等の見解を示すものではありません。制度改正や実務上の取扱いの変更等により、内容が最新でなくなる場合があります。実際の判断にあたっては、個別の状況に応じて専門家または関係機関にご確認ください。
