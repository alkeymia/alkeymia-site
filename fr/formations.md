---
title: Nos formations
navigation: Formations
weight: 4
---

<!-- Portfolio Start -->
<section id="portfolio-work">
    <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="block">
              <div class="portfolio-contant">
                <ul id="portfolio-contant-active">
                    {% for formation in site.formations %}
                    {% if formation.path contains page.lang %}
                    <li class="mix {{ formation.level }}">
                      <a href="{{ formation.url }}">
                        <img src="{{ site.baseurl }}/assets/formations/{{ formation.title }}.png" alt="">
                        <div class="overly">
                            <div class="position-center">
                              <h2>{{ formation.title }}</h2>
                              <p>{{ formation.description | strip_html | truncatewords: 30 }}</p>
                            </div>
                        </div>
                      </a>
                    </li>
                    {% endif %}
                    {% endfor %}
                </ul>
              </div>
            </div>
          </div>
        </div>
    </div>
</section>

{% include list-works.html %}
