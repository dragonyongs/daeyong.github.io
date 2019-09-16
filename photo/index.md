---
layout: default
work: true
main: true
title: Photo recommendation
description: 현재까지 촬영한 셀렉트 사진
project-header: true
header-img: "img/project_bg.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.photo == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
