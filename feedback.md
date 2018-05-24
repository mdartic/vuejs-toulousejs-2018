---
title: Meetup Vue.js Toulouse 24/05/2018
verticalSeparator: ------
---

<!-- .slide: data-background="./assets/vuejs-logo.png" class="bg-size-contain"  -->

# Vue.js

## Feedback Artl@s / Clearance

Retour d'expérience sur projets Vue.js professionnels

Mai 2018

---

<!-- .slide: data-background="./assets/artlas_logo.svg" class="bg-size-contain"  -->

------

# Projet Artl@s
# (2017-2018)

http://artlas.ens.fr/artlas_interface/visu/#/

http://artlas-staging.surge.sh/#/

------

## Équipe

* **2 dévs front** *@makina*
  * 1 junior en Vue.js avec expériences précédentes en Angular.js, React
  * 1 maîtrise en Vue.js avec expériences précédentes en Angular.js, React
* 1 dév back *@artlas* pour l'API

* **60 jours de dév front** commencés en 2017, en cours de finalisation

------

## Choix de Vue.js ?

Projet de taille modérée permettant une prise de risque tout aussi modérée

Volonté de découvrir sur projet professionnel le comportement de la lib

------

## Stack Vue.js

* CLI 2 (non migré sur 3)
* [vue-router](https://router.vuejs.org/)
* [Element](http://element.eleme.io/)
* [Vuex](https://vuex.vuejs.org/)
* [vue-i18n](https://kazupon.github.io/vue-i18n/)
* [leaflet](http://leafletjs.com/)
* [Plotly](https://plot.ly/javascript/)

Pas de SSR

------

## Feedback (les +)

* rapidité de prise en main par le dév débutant en Vue.js
* pas de blocage durant le développement propre à Vue.js
* TTM très rapide avec le framework graphique Element
* intégration avec leaflet & plotly sans souci

------

## Feedback (les -)

* catastrophique au niveau de l'écriture des tests
* debug des fichiers `.vue` peu confortable
* `console.log` des getter/setter sous Firefox pénible...
* attention à la structuration du store
  * entre les actions / mutations, on peut s'y perdre si on est pas assez rigoureux
  * surtout lors de la reprise du projet après 6 mois d'inactivité

Note:
tests : pas de jest à l'époque
debug: décalage des breakpoints

------

## Si c'était à refaire ?

* les tests se sont grandement améliorés avec `jest`, `vue-jest` ainsi que le projet `vue-test-utils`

* le debugger des getter/setter est peu fréquent, et Chromium/Chrome savent les gérer

donc, oui !

---

# Projet Clearance
# (2018)

------

## Équipe

* **2 dév back Django Rest Framework** partagé *@makina*/*@clearance*
* **1 dév fullstack junior** *@clearance* en Vue.js / DRF
* **1 dév front** *@makina*

**25 jours de front** (36 jours en tout), reste 10 jours actuellement (projet en cours)

------

## Choix de Vue.js ?

Demande du client
* considère qu'il n'a pas un grand niveau en JavaScript
* considère que Vue.js répond à une population habituée à du jQuery
souhaitant améliorer la construction de leurs applications

------

Côté Makina

Validation du choix technique du client
au vue de son projet et du temps qu'il pourra consacrer au code front

Ressource disponible sur Vue.js dans les temps requis par le client

------

## Stack Vue.js

* CLI 3
* [vue-router](https://router.vuejs.org/)
* [Vuetify](http://vuetifyjs.com/)
* [Vuex](https://vuex.vuejs.org/)
* [vue-gettext](https://github.com/Polyconseil/vue-gettext)
* [mapbox-gl](http://leafletjs.com/)

Pas de SSR

------

## Feedback (les +)

* pas de blocage durant le développement propre à Vue.js
* TTM très rapide avec le framework graphique Vuetify
* mise en place progressive du store
* code review par le client pour la partie front adaptée
* écriture des tests en jest agréable, avec les snapshots
* intégration sans souci avec mapbox-gl

------

## Feedback (les -)

* vue-gettext moins facile à appréhender que vue-i18n
* debug des fichiers `.vue` pas évident, décalage des breakpoints
* `console.log` des getter/setter sous Firefox pénible...

------

## Si c'était à refaire ?

Le projet n'est pas fini,
j'attends de voir la prise en main du client sur le code front.

Néanmoins, l'expérience développeur est encore une fois très agréable.

donc, oui !


---

<!-- .slide: data-background="./assets/vuejs-wallpaper.jpeg" -->

# Merci à tou-te-s
