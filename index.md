---
layout: default
title: Home
---

<section class="intro">
  <div class="container">
    <h2 class="intro__title">Thinking about service design</h2>
    <!-- <p class="intro__description">
      Inside Out delivers practical, engaging workshops to help designers and researchers grow their skills and make meaningful impact.
    </p> -->

  </div>
</section>

<section class="">
  <div class="container">
    <ul class="blog__posts">
      {% for post in site.posts reversed %}
        <li class="blog__post">
          <h3 class="blog__title"><a class="blog__link" href="{{ post.url }}">{{ post.title }}</a></h3>
          <time class="blog__date">{{ post.date | date: "%B %d, %Y" }}</time>
          <!-- <p class="article-list__excerpt">{{ post.excerpt }}</p> -->
          <p><a href="{{ post.url }}">Continue reading</a></p>
        </li>
      {% endfor %}
    </ul>
  </div>
</section>