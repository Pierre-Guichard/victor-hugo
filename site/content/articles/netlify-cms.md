---
title: Netlify CMS
tags:
  - Netlify CMS
thumbnail: https://upload.wikimedia.org/wikipedia/commons/d/d4/Netlify_CMS_logo.svg
---
Netlify CMS est une single page app javascript, qui offre un système d'édition et de gestion de fichiers Markdown.

Netlify CMS peut être utilisé indépendamment de [Netlify](/articles/netlify)

## Pour ?

L'app est délivrée via un CDN. Il n'y a rien à installer.

L'installation dans un projet est simple, il suffit de configurer les types de contenus voulus et les types de champs qui s'y rapportent au format YAML

![Configuration YAML](img/capture-d’écran-2022-11-18-154631.png "Configuration YAML")

Il possède un éditeur Rich text et un éditeur markdown pour certain champs.
L'upload des images est facilitée par l'éditeur Rich Text.

![Edition d'un article](img/capture-d’écran-2022-11-18-154802.png "Edition d'un article")

A chaque édition d'un contenu, un commit est envoyé sur le repo précisé dans la configuration (Avec une autorisation de l'app via OAuth pour l'accès au repo GitHub)

Dispose d'un système de brouillons, et de publication pour gérer les versions des articles.
## Contre ?
Si on modifie un élément lié à plusieurs fichiers markdown, il faudra modifier sur chacun des fichiers qui y fait appel: Si on modifie le nom d'un article, le slug sera modifié. Il faudra modifier le slug sur tous les autres articles y faisant appel à la main.

Options de back end limitées à l'utilisation des markdowns.

Pas de contenu dynamique

Doit être lié à un système de VCS hébergé (GitHub, GitLab, BitBucket...)