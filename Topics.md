---
layout: home
title: Categories02
permalink: /categories02/
---

{% for cat in site.categories %}


### {{ cat[0] }}

{% for post in site.posts %}
{% if post.category == cat[0] %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endif %}
{% endfor %}

{% endfor %}