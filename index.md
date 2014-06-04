---
layout: page
title: Load.List.Run.
tagline: A developers daily thoughts
---
{% include JB/setup %}

{% for post in site.posts %}
   <article>
      <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      <small>{{ post.date | date_to_string }}</small></h2>

      {{ content }}
   </article>
{% endfor %}
