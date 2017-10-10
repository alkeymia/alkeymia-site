Bonjour Betrand,


## 1ère phase:
 
* page home : 
 [X] le bouton "Programmes" doit linker vers la page Formations
 [X] les 3 formations proposées doivent linker vers la page de la formation correspondante

* page contact : 
 [X] formulaire : le message doit etre envoyé à l'adresse : contact@alkeymia.com (via formspree) 
 [X] spécifier comme adresse : 12 avenue Andrée, 94100 Saint-Maur-des-Fossés (la parametrer sur la carte google map aussi)
 [X] spécifier comme email : contact@alkeymia.com (linkable)
 [X] spécifier comme Téléphone  : +33 1 76 54 56 82
 [X] traduire "Shop for a visit par" "Coordonnées"
 [X] traduire "We Also Count In Google Map" par "Le Siège"
 [X] conserver que les liens sociaux Linkedin et Twitter (linker) . le lien Linkedin sera fourni plus tard.
 [X] remplacer la section "We design delightful digital experiences" par la meme section "Notre Métier" (qui est sur la home)

* page formations:
 [X] quand on a selectionné une formation, en plus de proposer l'ensemble des dates, proposer un lien "Prise de contact" qui linke aussi vers le formulaire, mais sans date initialisée. (mettre "A définir" au lieu de la date normalement affichée)
 [X] dans le formulaire d'inscription, ajouter des champs "Votre Prénom", " Votre Téléphone", Votre téléphone", "Votre besoin" (dans le meme ordre que https://training.zenika.com/contact)
 [X] la soumission du formulaire d'inscription doit envoyer un mail à training@alkeymia.com
 [X] sur chaque page de formation, comme sur la page https://training.zenika.com/formations/elasticsearch, prevoir un bloc à droite avec les liens "Formation au format PDF, Bulletin d'inscription, etc". (pour les fichiers PDF, linker vers des fichiers locaux, existants mais fictifs pour l'instant).

* page blog:
 [X] garder que le post "Welcome to jekyll!"

* général:
 [X] lien Twitter du footer : linker vers https://twitter.com/AlkeymiaEng
 [X] dans le header, déplacer le lien Blog entre Formations et Contact
 [0] Affichage de sections du site dans les résultats Google
 [0] mettre d’ores et déjà le site en ligne en https avec les redirections de domaine, en .com pour l'instant, spécifiées dans le cahier des charges
 [X] dans le header, afficher un selecteur de langue (Francais / Anglais), gestion par cookie. Le choix séléctionné doit surcharger la gestion auto faite selon la langue du browser. 
 [X] afficher le message d'avertissement "En poursuivant votre navigation sur notre site internet..." , et gérer l'acceptation par cookie
	> The cookie law is not actually about cookies (and its not actually called the cookie law). Its about tracking users, storing and sharing the information with third parties. Cookies are just the most popular method to track users.
		If you don't want to show the "cookie warning" then just don't track the users beyond the session and don't share traffic data with third parties.
		https://softwareengineering.stackexchange.com/questions/290566/is-localstorage-under-the-cookie-law
 [0] responsive : verifier l'affichage sur tablette et tel, il y a quelques problemes d'affichage de l'image du slider de la home par exemple.

Header site:
[X] ajouter un espace vertical (actuellement, les logos et liens du header sont collés tout en haut)

Footer site:
[X] mettre le lien twitter en target=”_blank”

favicon site:
[X] prendre le A du logo Alkeymia. (je le mettrai à jour de mon coté plus tard)

mention copyright
[X] possible de mentionner à la fois l’auteur du template et alkeymia?

Page Formation:
[X] remplacer le bloc “We design delightful digital experiences.” par le meme “Notre metier” (qui est sur la home)
[X] pour rappel, chaque page (elasticsearch, etc.) decrivant une formation doit afficher un bloc comme sur https://training.zenika.com/formations/elasticsearch:

[X] corriger le lien : formations/elestisearch/ en formations/elastisearch/
[X] dans la page formations/elestisearch/, remplacer les 2 mentions à “Kafka” par “Elasticsearch” (dans 2 sections à la fin)
[X] dans la page formations/cassandra, retirer toute la section “Ivan Beauvais”, corriger la coquille “Big Dat” en “Big Data”
[X] la soumission de formulaire de formation n’est pas fonctionnel (meme pb que pour la page contact)

Article de blog:
[X] tu as laissé cela: twitter. (twitter étant linkable vers le compte twitter https://twitter.com/AlkeymiaEng)
=> transformer en lien : twitter
[X] possible de mettre la date du post au format FR : JJ/MM/AAAA?

Page Notre métier:
[0] probleme d’agencement des images sur mobile/tablette :

=> L’image des 2 imacs devrait se trouver en dessous du texte “Formateurs passionnés”
Essayer de corriger, sinon, si c’est pas possible car du au fait que l’image succède directement celle du pont au mode desktop, intervertir alors la position du paragraphe “Formateurs passionnés” (qui se retrouvera à gauche comme les autres sections) et l’image à droite.

Page contact:
[X] mettre les liens twitter et linkedin en target=”_blank”
[X] l’envoi de message n’est pas fonctionnel? 
