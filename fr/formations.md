---
title: Nos formations
navigation: Formations
weight: 2
---

<!-- Portfolio Start -->
<section id="portfolio-work">
    <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="block">
              <div class="portfolio-menu">
                <ul>
										<li class="filter" data-filter="all">Tout</li>
										{% for formation in site.formations %}
                    {% if formation.path contains page.lang %}
                    <li class="filter" data-filter=".{{ formation.level }}">{{ formation.level }}</li>
										{% endif %}
                    {% endfor %}
                </ul>
              </div>
              <div class="portfolio-contant">
                <ul id="portfolio-contant-active">
                    {% for formation in site.formations %}
                    {% if formation.path contains page.lang %}
                    <li class="mix {{ formation.level }}">
                      <a href="{{ formation.url }}">
                        <img src="{{ site.baseurl }}/assets/img/portfolio/work1.jpg" alt="">
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

<!-- Call to action Start -->
<section id="call-to-action">
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="block">
          <h2>We design delightful digital experiences.</h2>
          <p>Read more about what we do and our philosophy of design. Judge for yourself The work and results we’ve achieved for other clients, and meet our highly experienced Team who just love to design.</p>
          <a class="btn btn-default btn-call-to-action" href="#" >Tell Us Your Story</a>
        </div>
      </div>
    </div>
  </div>
</section>
