---
title: Meetup Vue.js Toulouse 24/05/2018
verticalSeparator: ------
---

<!-- .slide: data-background="./assets/vuejs-wallpaper.jpeg" -->

---

<!-- .slide: data-background="./assets/vuejs-logo.png" class="bg-size-contain"  -->

# Vue.js

## Un monstre du loch ness ?

Introduction à la librairie & Feedbacks

Mai 2018

---

<!-- .slide: class="icon"  -->

Vos Gentils Animateurs

||||
|---|---|---|
|![Juliane](./assets/juliane.jpg)|Juliane Blier @tactless7|[SchoolMouv](https://www.schoolmouv.fr/)|
|![Mathieu](./assets/mathieu.jpeg)|Mathieu Dartigues @mdartic|[MakinaCorpus](https://makina-corpus.com)|
||||

---


# De quoi on va parler ce soir ?

------

de Vue.js, à travers
* un peu d'histoire et quelques chiffres
* une petite-démo-rapide (promis)
* les concepts clés
* l'écosystème
* les échéances à venir

------

et surtout

------

5 feedbacks sur des projets divers *made with vuejs*

* @tactless7 projet Schoolmouv
* @nnodot projet/expérience "débutant"
* @val-bubbleflat appli modulaire
* @mdartic projets Artl@s / Clearance
* @marcelfalliere projet avec framework quasar

---

# De quoi on ne va pas parler ce soir ?

------

* de la guerre des frameworks...
* et du monstre du loch ness (snif)


---

# Quelques chiffres

------

## Dates clés (1)

* *2009* : Sortie de **l'iPhone 3GS**, **AngularJS**
* *2013* : Premiers essais de refactorisation d'AngularJS
* *2013* : Sortie de la 0.6, première release
* *2014* : Sortie de la 0.11
* *2015* : Sortie de la 1.0 Evangelion
* *2015* : Adoption par la communauté Laravel comme brique front de base

------

## Dates clés (2)

* *2016* : [Campagne Patreon](https://www.patreon.com/evanyou), Evan You full time
* *2016* : Refonte complète avec la 2.0 Ghost In The Shell (Virtual DOM)
* *2017* : 2.5 Level E avec prise en compte des PWA, SSR, async components...
* *2017* : VueConf en Pologne
* *2018* : VueConf qui se multiplient : Amsterdam, US, Barcelone...

Note:
2016 marque le début de l'envolée de la popularité de vue

------

## Une popularité GitHub toujours croissante

* [Bestof JS Last 3 Months](https://bestof.js.org/tags/framework/trending/last-3-months)
* [Bestof JS Last 12 Months](https://bestof.js.org/tags/framework/trending/last-12-months)
* Projet GitHub le plus starré en 2017
* Une centaine d'issue en cours de traitement
* à ce jour, +95000 stars

------

## Des entreprises 'reconnues' qui l'utilisent


|||
|---|---|
| Nintendo | [GitLab](https://about.gitlab.com/2016/10/20/why-we-chose-vue/) |
| Alibaba  | [Facebook](https://newsfeed.fb.com) |
| Adobe  | [Codeship](https://blog.codeship.com/consider-vuejs-next-web-project/) |
| ...  | ... |

[cf listing](https://github.com/vuejs/awesome-vue#enterprise-usage)

------

Bref.

Quelques indicateurs qui démontrent
un intérêt prononcé de la communauté pour cette librairie.

---

# petite-démo-rapide !

promis...

Note:

à voir
* v-bind
* v-if
* v-for
* composants Person
* v-model avec formulaire de personne éditable / supprimable
* vue-devtools



---

# Les concepts clés

------

## Approche composant

------

## Single File Component

un template + un script + un style

= un composant

------

<!-- .slide: data-background="./assets/vue-component.png" class="bg-size-contain"  -->

Note:

Possibilité d'utiliser du TypeScript en lieu et place du JS
du SCSS / PostCSS / Less dans la partie style, de les scoper

------

## Virtual DOM

------

## Rendu déclaratif
## Système de réactivité

------

<!-- .slide: data-background="./assets/reactivity.png" class="bg-size-contain"  -->

------

## API développée et limitée (1)

* *props* = données d'instanciation du composant
* *data* = state du composant
* *computed properties* avec gestion de cache
* *méthodes*
* les watchers *watch*
* le binding des styles (class / style)

------

## API développée et limitée (2)

* *directives*
  * le one-way data flow *v-bind*
  * conditional rendering *v-if / v-else / v-else-if*
  * list rendering *v-for*
  * les event *v-on*, @click, @keyenter...
  * les directives customs...
  * le two-way data binding *v-model* (pratique pour les forms...)
* les slots / mixins
* les transitions (=> animation)


------

## Developer Experience

* documentation claire, maintenue au fil des évolutions, traduite dans plusieurs langues
* comparatif entre frameworks sur la doc°
* breaking change peu nombreux, assistés en cas de migration
* courbe d'évolution très rapide

Note:
Vue.js est une bonne entrée en matière pour découvrir les frameworks JS

------

## Framework progressif ?

Note:
On parle de Vue.js comme étant le framework progressif / évolutif.

Pourquoi le framework progressif ?

------

<!-- .slide: data-background="./assets/vuejs-progressive-framework.png" class="bg-size-contain" -->

Note:
Chaque nouveau cercle (hormis les deux premiers) est une brique à ajouter au framework

---

# Ecosystème Vue.js

------

## Outillage

* *routing* : vue-router
* *store* : vuex, basé sur Flux
  * réflexion en cours sur la fusion des actions (asynchrones) et mutations (synchrones) par l'utilisation des async / await
* *translation* : vue-i18n, vue-gettext
* *tests* : vue-test-utils avec jest
* *debug* : vue-devtools

Note:
Vue-devtools sur Google Chrome et plus récemment sur Firefox

------

## [CLI 3.0-beta](https://github.com/vuejs/vue-cli/)

```sh
npm install -g @vue/cli

vue create my-project
```

* plusieurs choix / réutilisation d'un preset
  * TypeScript / Transpiler ES6/7/x / PWA
  * linters (StandardJS, ESLint)
  * preprocessors pour le style (sass / postcss)
  * test unitaires / d'intégrations
  * accepte le JSX
* fonctionne avec des plugins
* permet de conserver une évolutivité sans éjecter

Note:

cf démo

version finale

------

<!-- .slide: data-background="./assets/nuxtjs-logo.png" class="bg-size-contain"  -->

## [Nuxt.js](http://nuxtjs.org/)

  * Équivalent de next pour React
  * facilite la construction de projet Vue.js
  * SSR, SPA, sites statiques, ...
  * Split automatique du code selon les routes
  * Transpilation ES6/ES7

Note:
Il existe aussi vue-ssr (doc dans les repos officiels vue.js)

------

## Mobile

* [NativeScript-Vue](https://nativescript-vue.org/)

* [Weex](https://weex.apache.org/) (Apache Incubator, projet d'Alibaba initialement)

Note:
* Outils récents (sortie fin 2017/début 2018)
* Encore peu de retours sur leur utilisation

------

## Librairies graphique

* vuetify basé sur Material
* Element
* Bootstrap
* Quasar (cf feedback)

------

L'écosystème de Vue.js est en constante évolution,
mais il y a un socle qui définit le framework Vue.js
par l'adoption et la maintenance de briques essentielles
au delà de la simple librairie de composant qu'est Vue.js.

---

# État du projet

------

## Actuellement, début 2018

* sortie de nuxt 1.0 (maintenant 1.4), [NativeScript-Vue 1.0](https://nativescript-vue.org/), [vuetify 1.0](https://vuetifyjs.com/)
* évangélisation de vuejs à travers plusieurs conférences pour aller au contact des dévs

Note:
Projet communautaire, et financé par des campagnes Patreon
Core team réduite, contribution Evan You essentielle, mais stratégie de délégation de plus en plus présente
Communauté indispensable au développement des briques 'tierces', type nuxt, vue-test-utils, vue-devtools, vue-apollo, vue-i18n... traduction des documentation pour plus d'accessibilité (force du côté asiat, mais aussi france etc.)
Communauté FR présente : frères Chopin = Nuxt, Eduardo @posva (espagnol parisien), @akryum

Même un projet qui fait marcher du code React dans Vue & inversement (https://github.com/akxcv/vuera) !

Onboarding facile

------

## L'avenir proche pour 2018

* vue-cli 3.0 avec webpack 4 et vue-loader 15
* morceau extrait de vue-loader pour compat rollup / parcel / ?
* mise en place de la 2.6-next avec abandon support IE, utilisation des Proxy => plus de caveat pour le système de réactivité
* mise en place de RFC pour mieux diriger
* stabilisation de la librairie, travail sur les briques d'accompagnement

---

## Feedback

Constantes :

* taille du projet / équipe (nombre de jours / personnes)
* technos utilisées (front / back / tooling)
* pourquoi le choix de Vue.js
* avantages / inconvénients de l'utilisation de Vue.js
* si c'était à refaire ?

------

Les retours :

* @tactless7 projet Schoolmouv
* @nnodot projet/expérience "débutant"
* @val-bubbleflat appli modulaire
* @mdartic projet Clearance
* @marcelfalliere projet avec framework quasar

---
<!-- .slide: data-background="./assets/vuejs-logo.png" class="bg-size-contain"  -->

## En conclusion, Vue.js c'est...

------

Vue [...] est un framework évolutif
pour construire des interfaces utilisateur.
À la différence des autres frameworks monolithiques,
Vue a été conçu et pensé pour pouvoir être adopté
de manière incrémentale.
Le cœur de la bibliothèque est concentré uniquement
sur la partie vue, et il est vraiment simple
de l’intégrer avec d’autres bibliothèques ou projets existants.
D’un autre côté, Vue est tout à fait capable
de faire tourner des applications web monopages
quand il est couplé avec des outils modernes
et des bibliothèques complémentaires.

[source fr.vuejs.org](https://fr.vuejs.org/v2/guide/index.html#Vue-js-qu%E2%80%99est-ce-que-c%E2%80%99est)

---

# Quelques liens

* [Vue.js](https://vuejs.org)
* [Awesome Vue.js](https://github.com/vuejs/awesome-vue)
* [Vue.js News](https://news.vuejs.org/) avec podcast
* [Channel Discord](https://discordapp.com/channels/325477692906536972/360669119948783616)
* [Communauté traduction FR](https://gitter.im/vuejs-fr/vue)
* [VueConf New Orleans 2018](https://www.vuemastery.com/vueconf)

---

<!-- .slide: data-background="./assets/vuejs-wallpaper.jpeg" -->

# Merci à tou-te-s
