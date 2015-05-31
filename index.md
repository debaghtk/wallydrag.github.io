---
layout: page
title: Hello there!
tagline: Supporting tagline
---
{% include JB/setup %}

I really don't have any idea what to say to you here.
But now that you are here, you have browse around.

## Posts

This blog contains posts which help stage pages and blog data.
Here's "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
