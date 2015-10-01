---
title: "All Events"
layout: "page-w-col"
col_header: "Event Pages"
links:
  - link: "/git"
    title: "Git"
---

{% for post in site.categories.all %}
<div class="blog-post">
  <h2 class="blog-post-title">{{ post.title }} </h2>
  <p class="blog-post-meta">{{ post.date  | date: '%B %d, %Y' }}</p>
  <p class="blog-post-meta">{% if post.location %}{{ post.location }}{% else %}Location is not set yet{% endif %}</p>
  {{ post.excerpt }}
  <p>
  <a class="btn btn-primary btn-lg" href="{{ post.url }}" role="button">Read more »</a>
  </p>
</div>
{% endfor %}

<script type="text/javascript">
  $("#eventsnav").addClass("active");
</script>
