---
layout: archive
title: "Web"
permalink: /web/
author_profile: false
---

{% assign category = "Web" %}
{% assign posts = site.pages | where_exp: "post", "post.categories contains category" and "post.hidden != true" %}
{% for post in posts %}
{% include archive-single.html %}
{% endfor %}
