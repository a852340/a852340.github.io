---
layout: page
title: About
description: 一枚小小码农!~
keywords: Me
comments: true
menu: 关于
permalink: /about/
---

世上能做的事情很多

想做的事情也很多

只愿把眼前的事情做好

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
</ul>

## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
</ul>