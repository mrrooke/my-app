---
layout: post
title: Revision
---

Resources that may be helpful to you as you revise:

<ul>
{% assign published_posts = (site.revision | where:"list","true")  %}
{% for post in published_posts %}
    <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
