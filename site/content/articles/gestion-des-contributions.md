---
title: Gestion des contributions
tags:
  - Netlify CMS
  - Netlify
thumbnail: https://www.google.com/url?sa=i&url=https%3A%2F%2Fgiphy.com%2Fexplore%2Fcat-typing&psig=AOvVaw1iE_ltmFigcRxdX594lAUe&ust=1669122564287000&source=images&cd=vfe&ved=0CA8QjRxqFwoTCMCXhZ2sv_sCFQAAAAAdAAAAABAj
---
Les contributions sont gérées grâce à [Netlify CMS](/articles/netlify-cms).

## Autorisations

Les utilisateurs doivent disposer d'un compte GitHub. Il faut avoir accès au repo pour pouvoir accéder à la partie [admin](/admin).
L'application doit avoir un accès au repo sur le compte GitHub. (ajouter Netlify à [GitHub Apps](https://github.com/Pierre-Guichard/victor-hugo/settings/installations) + [Oauth](https://github.com/settings/developers))



Modification avec un autre compte

## Gestion des publications

Chaque nouvelle publication, ou chaque modification fait l'objet d'une branche. Chaque modification sauvegardée correspond à un commit.
Au moment de la publication, la branche créée pour la nouvelle publication et/ou ses modifications est mergée dans la branche dédiée à la publication (Modifiable dans le fichier yaml de config de [Netlify CMS](/articles/netlify-cms).

## Mise en ligne

À chaque nouveau commit sur la branche précisé ([Settings > Branch](https://app.netlify.com/sites/lively-cat-817b2d/settings/deploys)), la branche est par défaut déployée (Modifiable dans [Settings > Deploy Preview](https://app.netlify.com/sites/lively-cat-817b2d/settings/deploys))

## Sitemaps

Hugo donne la possibilité de générer automatiquement le [sitemap](/sitemap.xml). Il est paramétrable (cf [Doc](https://gohugo.io/templates/sitemap-template/))

## RSS

Des flux [Rss](/index.xml) peuvent être paramétrés avec Hugo et adaptés aux besoins