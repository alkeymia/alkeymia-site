---
title: Contactez us !
navigation: Contact
navigation_footer: Contact
weight: 10
---
<!-- contact form start -->
<section>
  <div id="form" class="container">
    <div class="row">
      <div class="block">
        <form action="https://formspree.io/contact@alkeymia.com" method="POST">
          <legend>{{ site.data.i18n.contact[page.lang].legend }}</legend>
          <div class="form-group">
            <label>{{ site.data.i18n.contact[page.lang].lastname}}</label>
            <input type="text" class="form-control" placeholder="ex: Jean Delafontaine" name="nom">
          </div>
          <div class="form-group">
            <label>{{ site.data.i18n.contact[page.lang].email}}</label>
            <input type="text" class="form-control" placeholder="ex: jean.delafontaine@mail.com" name="_reply">
          </div>
          <div class="form-group">
            <label>{{ site.data.i18n.contact[page.lang].subject}}</label>
            <input type="text" class="form-control" placeholder="ex: accès au lieu de formation" name="_subject">
          </div>
          <div class="form-group-2">
            <label>{{ site.data.i18n.contact[page.lang].message}}</label>
            <textarea class="form-control" rows="3" placeholder="J'ai un sujet à vous soumettre" name="message"></textarea>
          </div>
          <button class="btn btn-default" type="submit">{{ site.data.i18n.contact[page.lang].submit}}</button>
        </form>
      </div>
    </div>
  </div>
</section>
<section>
  <div class="container">
    <div id="contact-box" class="row">
      <div class="col-md-6 col-sm-12">
        <div class="block">
          <h2>Coordonnées</h2>
          <ul class="address-block">
            <li>
              <i class="fa fa-map-marker"></i>12 avenue Andrée, 94100 Saint-Maur-des-Fossés
            </li>
            <li>
              <i class="fa fa-envelope-o"></i>Email: <a href="mailto:contact@alkeymia.com">contact@alkeymia.com</a>
            </li>
            <li>
              <i class="fa fa-phone"></i>Téléphone: +33 1 76 54 56 82
            </li>
          </ul>
          <ul class="social-icons">
            <li>
              <a href="https://linkedin.com/alkeymia" target="_blank"><i class="fa fa-linkedin"></i></a>
            </li>
            <li>
              <a href="https://twitter.com/AlkeymiaEng" target="_blank"><i class="fa fa-twitter"></i></a>
            </li>
          </ul>
        </div>
      </div>
      <div class="col-md-6 col-sm-12">
        <div class="block">
          <h2>Le Siège</h2>
          <div class="google-map">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d5254.859280244906!2d2.4758768330453087!3d48.81186337928301!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e60ce19354f3df%3A0x56307f962fdc1d40!2s12+Avenue+Andr%C3%A9e%2C+94100+Saint-Maur-des-Foss%C3%A9s!5e0!3m2!1sfr!2sfr!4v1507184600140" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
