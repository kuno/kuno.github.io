---
layout: index
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

<ul>

{% for post in site.posts %}

<li>
 <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - <small>{{ post.date | date_to_string }}</small></li>

{% endfor %}

</ul>