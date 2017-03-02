---
layout: page
title: Archive
---

{% for post in site.posts %}{%unless post.layout == "micro" %}* {{ post.date | date: "%Y-%m-%d %H:%M" }} - [{{ post.title }}]({{ post.url }})
{% endunless %}{% endfor %}
