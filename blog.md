---
layout: page
title: Blog
permalink: /blog/
---

Welcome to my blog! In high school I created a website called TucánAyuda which provided college admissions advice for Costa Rican students. If you would like to learn more click [here](https://tucanayuda.com/). Now, in university, I would like to continue and share insights primarily about pursuing academic research at the undergraduate level.

<div class="blog-posts">
{% for post in site.blog %}
  <article class="blog-post-preview">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
  </article>
  <hr>
{% endfor %}
</div>

<style>
.blog-post-preview {
  margin-bottom: 2rem;
}

.blog-post-preview h3 {
  margin-bottom: 0.5rem;
}

.blog-post-preview h3 a {
  text-decoration: none;
  color: inherit;
}

.blog-post-preview h3 a:hover {
  text-decoration: underline;
}

.read-more {
  color: #0066cc;
  text-decoration: none;
  font-weight: 500;
}

.read-more:hover {
  text-decoration: underline;
}

hr {
  margin: 2rem 0;
  border: none;
  border-top: 1px solid #eee;
}
</style>