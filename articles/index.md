---
layout: page
---

# Articles

{% for article in site.categories.articles %}
<div class="blog-post">
  <h2 class="blog-post-title">{{ article.title }} </h2>
  <p class="blog-post-meta">{{ article.date  | date: '%B %d, %Y' }} • Author: <strong>{{ article.author }}</strong></p>
  {{ article.excerpt }}
  <p>
  <a class="btn btn-primary btn-lg" href="{{ post.url }}" role="button">Read more »</a>
  </p>
</div>
{% endfor %}
