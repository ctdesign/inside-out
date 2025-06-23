---
layout: default
title: Home
---

<section class="intro">
  <div class="container">
    <h2 class="intro__title">Making service design work for you</h2>
    <p class="intro__description">
      Inside Out delivers practical, engaging workshops to help designers and researchers grow their skills and make meaningful impact.
    </p>
  </div>
</section>

<section class="">
  {% for post in site.words reversed %}
    <li class="article-list__item">
      <p class="meta">Posted on {{ post.date | date: "%B %d, %Y" }}</p>
      <h3 class="article-list__title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="article-list__excerpt">{{ post.excerpt }}</p>
      <p><a href="{{ post.url }}">Continue reading</a></p>
    </li>
  {% endfor %}
</section>