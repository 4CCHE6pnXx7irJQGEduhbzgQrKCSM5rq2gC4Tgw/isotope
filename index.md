---
layout: default
---

<div class="posts">
  {% for post in site.posts %}
    <p><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> <small><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time></small></p>
  {% endfor %}
</div>