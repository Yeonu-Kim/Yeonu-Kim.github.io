---
layout: archive
title: "Computer Science"
permalink: /computer-science/
author_profile: false
---

{% assign category = "CS" %}
{% assign posts = site.pages | where_exp: "post", "post.categories contains category" and "post.hidden != true" %}
{% for post in posts %}
{% include archive-single.html %}
{% endfor %}
