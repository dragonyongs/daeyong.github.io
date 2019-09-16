---
layout: default
work: true
main: true
title: Book recommendation
description: 읽을만한 책 추천!
project-header: true
header-img: "img/book_bg.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.book == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
