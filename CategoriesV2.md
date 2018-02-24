---
layout: home
title: Categories (V2)
permalink: /categoriesV2/
---

{% for cat in site.categories %}


### {{ cat[0] }}

{% for post in site.posts %}
{% if post.category == cat[0] %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endif %}
{% endfor %}

{% endfor %}