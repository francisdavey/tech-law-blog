---
title: Welcome page
layout: default
---

{% for post in site.posts %}
<span class="longdate">{{ post.date | date: "%A %e %B %Y" }}</span>
<h2 class="post-title"><a href="{{ post.permalink }}">{{ post.title }}{% if post.subtitle %} - {{post.subtitle}}{% endif %}</a></h2>

<p>{{ post.content }}</p>
{% endfor %}
