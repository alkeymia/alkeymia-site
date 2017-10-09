---
title: Accueil
description: Implémentation de solutions orientées ROI, DEVOPS, à l'état de l'art technologique
permalink: /fr/
navigation: Accueil
weight: 1
---

<!-- Slider Start -->
<section id="slider">
  <div class="container">
    <div class="row">
      <div class="col-md-10 col-md-offset-2">
        <div class="block">
          <h1 class="animated fadeInUp">CRÉATEUR DE SOLUTIONS <br> SUR MESURE</h1>
          <p class="animated fadeInUp">Implémentation de solutions orientées ROI, DEVOPS, à l'état de l'art technologique
            </p>
        </div>
      </div>
    </div>
  </div>
</section>
<!-- Wrapper Start -->
<section id="intro">
  <div class="container">
    <div class="row">
      <div class="col-md-7 col-sm-12">
        <div class="block">
          <div class="section-title">
            <h2>Nos atouts</h2>
            <p>Culture de l'innovation, mutualisation des connaissances.</p>
          </div>
          <p>Sur le plan technique, nous avons construit une puissante librairie de code au travers de tous nos déploiements. Chacune de ses parties nous permet de développer plus rapidement, efficacement et durablement. En matère de recrutement, notre stratégie de développement s'appuie, depuis 10 ans, sur une croissance mesurée et maîtrisée des équipes. Nous avons choisi de travailler sur une intégration spécifique et réussie de nos collaborateurs afin de les accompagner tout au long de leur carrière sur le choix des missions et leurs formations. Cela vous garantit un processus de recrutement personnalisé prenant en compte vos compétences, mais aussi votre potentiel et vos attentes spécifiques. Nous examinons, de la même façon, toute offre de collaboration même si votre profil ne correspond pas à 100 % aux profils décrits dans les annonces. D'une manière générale, notre travail est toujours réalisé en transparence et convenu en amont tant sur les jalons que sur les coûts. Les budgets sont régulièrement contrôlés durant les phases projets afin de garantir leurs utilisations optimales.</p>
        </div>
      </div><!-- .col-md-7 close -->
      <div class="col-md-5 col-sm-12">
        <div class="block">
          <img src="/assets/img/wrapper-img.png" alt="Img">
        </div>
      </div><!-- .col-md-5 close -->
    </div>
  </div>
</section>

<section id="feature">
<div class="container">
  <div class="row">
    <div class="col-md-6 col-md-offset-6">
      <h2>BigData</h2>
      <p>Notre cœur de métier est le Big Data. Grâce à une équipe de R&D, nous consacrons notre énergie et nos technologies à accompagner nos clients jusqu’au bout dans la mise en place de stratégies et d’exécution digitale. Nous proposons aussi des formations sur des technologies gravitant dans cet écosystème.</p>
      <a href="/{{ page.lang }}/formations/" class="btn btn-view-works">Programmes</a>
    </div>
  </div>
</div>
</section>

<!-- Service Start -->
<section id="service">
  <div class="container">
    <div class="row">
      <div class="section-title">
        <h2>Nos Formations</h2>
      </div>
    </div>
    <div class="row">
      {% for formation in site.formations %}
      {% if formation.path contains page.lang %}
      <div class="col-sm-6 col-md-4">
        <div class="service-item">
          <a href="{{ formation.url }}"><img src="{{ site.baseurl }}/assets/formations/{{ formation.title }}.png" alt="{{ formation.title }}"></a>
          <p>{{ formation.description | strip_html | truncatewords: 30 }}</p>
        </div>
      </div>
      {% endif %}
      {% endfor %}
    </div>
  </div>
</section>

{% include list-works.html %}


