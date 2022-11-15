---
layout: default
page_id: 'home.manual'
group_id: home
lang: zh-CN
title: '用户手册'
---
{% include_relative ManualInclude_Head_cn.md %}

{% assign pages = site.data.manual.pages | where: "lang", page.lang %}
{% for p in pages %}
  <h4><a href="{{ site.home.url }}/{{ p.pattern }}">{{ p.text }}</a><h4>
{% endfor %}
