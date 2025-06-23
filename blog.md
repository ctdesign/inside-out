---
layout: default
title: Blog
permalink: /blog/
---

<section class="blog__list">
  <div class="container">
    <h2 class="blog__title">Latest Blog Posts</h2>
    <ul class="blog__posts">
      {% for post in site.posts %}
        <li class="blog__post">
          <a class="blog__link" href="{{ post.url }}">{{ post.title }}</a>
          <time class="blog__date">{{ post.date | date: "%B %d, %Y" }}</time>
        </li>
      {% endfor %}
    </ul>
  </div>
</section>
