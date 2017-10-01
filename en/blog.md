---
title: Blog
navigation: News
weight: 2
---
<!-- Slider Start -->
<section id="global-header">
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="block">
          <h1>Get the latest on what we're doing</h1>
          <p>Catch up with us, anytime and anywhere</p>
        </div>
      </div>
    </div>
  </div>
</section>
{% for post in site.posts %}
{% if post.path contains page.lang %}
<div class="post-area">
  <a href="{{ post.url | prepend: site.baseurl }}" class="bold">{{ post.title }}</a>
  <p class="post-date">{{ post.date | date_to_long_string }}</p>
  <p>
    {{ post.content | strip_html | truncatewords: 50 }}
  </p>
</div>
{% endif %}
{% endfor %}