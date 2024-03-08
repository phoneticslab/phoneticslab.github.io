---
layout: default
title: news
permalink: /news/
---

# news

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})

{{ post.content | strip_html | truncatewords: 50 }}
[Read more]({{ post.url }})

{% endfor %}