---
title: Nos actualités
navigation: Blog
navigation_footer: Blog
weight: 9
---
<!-- Slider Start -->
<section id="global-header">
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="block">
          <h1>{{ page.title }}</h1>
        </div>
      </div>
    </div>
  </div>
</section>
{% for post in site.posts %}
{% if post.path contains page.lang %}
<div class="post-area container container-narrow">
  <a href="{{ post.url | prepend: site.baseurl }}" class="bold">{{ post.title }}</a>
  <p class="post-date">{{ post.date | date: "%D" }}</p>
  <p>
    {{ post.content | strip_html | truncatewords: 50 }}
  </p>
</div>
{% endif %}
{% endfor %}
