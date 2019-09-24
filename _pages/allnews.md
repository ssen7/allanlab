---
title: "News"
layout: textlay
excerpt: "Gut AI"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em>
<img src='{{ site.baseurl }}/images/news/{{article.image}}' class='img-responsive' style='{{article.style}}' />
</p>
{% endfor %}
