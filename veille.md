---
layout: default
title: Veille
---

La veille technologique consiste à surveiller les évolutions techniques, les innovations dans un secteur d’activité donné. La veille technologique comprend notamment la surveillance, la collecte, le partage et la diffusion d’information dans le but de les analyser et ainsi faire apparaitre des tendances et des corrélations. L’analyse des données collectées permet d’anticiper et de s’informer sur les changements en matière de recherche et développement.

## I. Présentation du Wifi

## II. Tri et sélection d'articles en rapport avec le Wifi

## III. Evolution de Wifi : le Wifi 6

`## Historique des articles :

{% assign postsByYearMonth = site.posts | group_by_exp: "post", "post.date | date: '%B %Y'" %}
{% for yearMonth in postsByYearMonth %}
  <h2>{{ yearMonth.name }}</h2>
  <ul>
    {% for post in yearMonth.items %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}`
