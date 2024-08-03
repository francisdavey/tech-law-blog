---
title: Welcome page
layout: default
---

{% for post in site.posts %}
<span>{{ post.date | date: %W %d %M %Y}}</span>
<h2 class="post-title"><a href="{{ post.permalink }}">{{ post.title }}{% if post.subtitle %} - {{post.subtitle}}{% endif %}</a></h2>

<p>{{ post.content }}</p>
{% endfor %}
