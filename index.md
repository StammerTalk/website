---
layout: default
---

<div id="posts-container">

  {% for post in site.posts %}
    <article>
      <h2>{{ post.title }}</h2>
      <p>{{ post.content }}</p>
    </article>
  {% endfor %}
</div>