---
layout: default
title: Historique
---

# Télétravail

La veille technologique consiste à s'informer en continu sur les nouveautés du secteur informatique, les inventions des concurrents ainsi que les nouvelles technologies et ce dans le but d'être le meilleur dans son domaine.

- VPN
- Outils de gestion à distance

# Historique des articles :

{% assign postsByYearMonth = site.posts | group_by_exp: "post", "post.date | date: '%B %Y'" %}
{% for yearMonth in postsByYearMonth %}
  <h2>{{ yearMonth.name }}</h2>
  <ul>
    {% for post in yearMonth.items %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
