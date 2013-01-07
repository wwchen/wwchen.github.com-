---
layout: page
title: William Chen
tagline: Jotting down tidbits as I learn them
---
{% include JB/setup %}

## Recent Posts

<ul class="posts">
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      <div>{{ post.content | strip_html | truncatewords: 100 }}</div>
    </li>
  {% endfor %}
</ul>

