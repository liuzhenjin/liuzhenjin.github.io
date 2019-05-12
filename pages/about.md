---
layout: page
title: About
description: 从零开始构建世界
keywords: Zhenjin Liu, 刘振进
comments: true
menu: 关于
permalink: /about/
---

从零开始构建世界。

仰慕「优雅编码的艺术」。

用心感受代码之美。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
