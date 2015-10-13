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
  {% if post.subtitle %}<h4 class="blog-post-meta">{{ post.subtitle }}</h4>{% endif %}
  {% if post.event %}{% else %}<p class="blog-post-meta">{% if post.location %}{{ post.location }}{% else %}Location is not set yet{% endif %}</p>{% endif %}
  <p class="blog-post-meta">{{ post.date  | date: '%B %d, %Y' }}{% if post.event %} at {% if post.time %}{{ post.time }}{% else %}{{ site.data.basicinfo.event_base_time }}{% endif %} in {% if post.room %}{{ post.room }}{% else %}{{ site.data.basicinfo.event_base_room }}{% endif %}{% endif %} • Category: <strong>{{ post.categories | last }}</strong></p>
  {{ post.excerpt }}
  <p>
  <a class="btn btn-primary btn-lg" href="{{ post.url }}" role="button">Read more »</a>
  </p>
</div>
{% endfor %}

<script type="text/javascript">
  $("#eventsnav").addClass("active");
</script>
