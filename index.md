---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

{% if site.posts.size == 0 %}
  <h2>No posts found</h2>
{% else %}
  {% for post in site.posts %}
  <div class="content list">
    <div class="list-item">
      <h2 class="list-post-title">
        <a href="{{ site.baseurl | append: post.url }}">{{ post.title }}</a>
      </h2>
      <div class="list-post-date">
        <time>{{ post.date | date_to_string }}</time>
      </div>
    </div>
  </div>
  {% endfor%}
{% endif%}
