---
layout: page
title: Thyphoon's Blog
tagline: Beautiful code has its source in great companies
---
{% include JB/setup %}

<div class="articles">
  {% for post in site.posts %}
  <article>
    <h1 class="emphnext"><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h1>

    {{ post.content }}

    <div class="disqus_comment_count">
      <a href="{{ BASE_PATH }}{{ post.url }}#disqus_thread" data-disqus-identifier="{{ page.url }}">See Comments</a>
    </div>
    
  </article>


  {% endfor %}
</div>

