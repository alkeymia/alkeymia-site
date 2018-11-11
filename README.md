# Alkeymia
Implémentation de solutions orientées ROI, DEVOPS, à l'état de l'art technologique

## Jekyll

Jekyll est un générateur de site statique Open Source écrit en Ruby([https://jekyllrb.com](https://jekyllrb.com)). 

**Architecture des répertoires :**
```
_data       # Fichiers YML
_formations # Fichiers markdown des formations
_includes   # Blocs de code appelés dans différentes pages
_layouts    # Gabarits des pages
_posts      # Billets de Blog
_sass       # Fichiers de styles compilé en Sass
_sessions   # Fichiers des sessions en lien avec une formation
admin	      # Répertoire pour Netlify CMS
assets      # Fichiers ressources : imahes, css, favicons…
en          # Pages en anglais
fr          # Pages en français
```

**Architecture des fichiers à la racine :**
```
.gitignore  # Fichier d'exclusion pour git
Gemfile     # Déclaration des plugins Jekyll
_config.yml # Configuration générale
index.html  # Pages d'accueil
LICENSE.md  # License
README.md   # Explicatif de fonctionnement
```

## Édition

Le contenu du site se modififie en grande partie dans des fichiers Markdown. Ces fichiers ont une extension en .md.

Comme Jekyll ne gère pas nativement les sites multilingues, les url en français et en anglais sont la conséquence d'une configuration et les fichiers de contenus sont répartis dans des répertoires différents.

### Formations

Formation est une collection. Les fichiers de formations sont présents dans le répertoire _formations à la racine.
Les langues sont complétements indépendantes, mais doivent être identiques pour les redirections automatiques par langue.

```
_formations
en
  cassandra.md
  elasticsearch.md
  kafka.md
fr
  cassandra.md
  elasticsearch.md
  kafka.md
```

Dans chaque répertoire de langue, il est possible d'ajouter autant de formation que souhaité. Le nom de fichier sert au référencement (url). Il doit être unique.

Pour créer une formation, créer un fichier avec le nom de son choix (ex: mongoDB.md). Et ajouter l'image correspondante dans : assets/formation/.

```
---
title: Cassandra # Titre qui s'affichera sur la page et identifiant pour la relation avec les sessions (attention aux majuscules)
excerpt: "presentation de l'architecture NoSQL, topologies des clusters, interrogation et mise à jour, administration" # Résumé, affiché sur le blocs de la page d'acceuil, sert pour le référencementet les réseaux sociaux
image: /assets/formations/cassandra.png
---
```

### Sessions

Les sessions sont au même titre que les formations une collection. Ils ont le même fonctionnement sauf qu'il n'y a pas d'image à gérer.

Pour créer une formation, créer un fichier avec le nom de son choix en ajoutant une date pour différencier chaque session (ex: mongoDB-21-mars-2042.md).

```
---
title: Cassandra	# Titre de la session doit être identique à celui de la formation ((attention aux majuscules))
session: lundi 26 mars 2018 - mercredi 28 mars 2018 # Période
duration : 3 jours # Durée
code-formation: cassandra # Code formation (pour le moment redondant avec le titre)
price: 1390 euros HT	# Prix
date-session: 2018-03-26 # Date au format Jekyll
---
```

Les sessions dont la date est dépassée ne s'affichent plus. Mais la page existe toujours. Pour supprimer la page, il est nécessaire de supprimer le fichier de formation.

**Les sessions sans date**

Il est possible de créer des formulaires de contact avec les informations de sessions mais sans date. Le principe est le même que pour une session avec date, mais il faut ajouter le paramètre __simplecontact__.
Ce paramètre affiche un lien à une position différente sur la page.

```
---
title: Cassandra
simplecontact: true
---
```

### Textes intertionalisés

Pour éviter de dupliquer du code dans des pages anglais et fançais. Un fichier i18n.yml existe dans le répertoire _data. Il liste les variables de langues qui s'affichent dans différents blocs (_includes principalement) ou pages (contact.md).

Les variables sont déjà créées dans le fichier, simplement remplacer les valeurs anglaises. (Il peut en manquer)

```
header:
  en:
    title: CRÉATEUR DE SOLUTIONS <br> SUR MESURE
    slogan: Implémentation de solutions orientées ROI, DEVOPS, à l'état de l'art technologique
  fr:
    title: CRÉATEUR DE SOLUTIONS <br> SUR MESURE
    slogan: Implémentation de solutions orientées ROI, DEVOPS, à l'état de l'art technologique
```

## Le référencement (SEO)

Un plugin de gestion des metadata est présent. Les valeurs sont remplies automatiquement en fonction de valeurs remplies dans les fichiers.

Le plus important est de bien nommer les fichiers. Les noms de fichiers servent à l'écriture des URL.
Pour le reste, c'est la qualité du code est du contenu brut qui va jouer pour le référencement.

### Installation

sudo apt-get -y install screen build-essential libpcre3-dev libssl-dev make zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget llvm libncurses5-dev

sudo apt-get -y install ruby-dev zlib1g-dev liblzma-dev

sudo gem install jekyll

sudo gem install bundler

sudo gem install html-proofer

sudo gem install jekyll-sitemap

sudo gem install jekyll-feed

sudo gem install jekyll-seo-tag

sudo gem install jekyll-github-metadata

sudo gem install jekyll-default-layout

sudo gem install jekyll-redirect-from

bundle exec jekyll serve

## Rafraichissement manuel

bundle exec jekyll clean

bundle exec jekyll build


