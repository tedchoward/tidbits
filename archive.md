---
layout: page
title: Archive
---

{% for post in site.posts %}* {{ post.date | date: "%Y-%m-%d %H:%M" }} - [{{ post.title }}]({{ post.url }})
{% endfor %}
