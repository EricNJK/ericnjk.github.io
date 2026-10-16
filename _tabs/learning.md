---
# the default layout is 'page'
#layout: home
icon: fas fa-info-circle
title: Learning
order: 5
# show links to all posts + preview 
---

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <time>{{ post.date | date: "%Y-%m-%d" }}</time>
    <div>{{ post.excerpt }}</div>
  </article>
{% endfor %}
