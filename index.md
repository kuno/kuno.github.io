---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

<p>最新文章</p>

<ul>

{% for post in site.posts %}

<li>
 <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - <small>{{ post.date | date_to_string }}</small></li>

{% endfor %}

</ul>