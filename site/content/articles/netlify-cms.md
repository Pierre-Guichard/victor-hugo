---
title: Netlify CMS
tags:
  - Netlify CMS
---
Netlify CMS est une single page app javascript, qui offre un système d'édition et de gestion de fichiers Markdown.

# Pour ?

L'app est délivrée via un CDN. Il n'y a rien à installer.

L'installation dans un projet est simple, il suffit de configurer les types de contenus voulus et les types de champs qui s'y rapportent au format YAML

![Configuration YAML](img/capture-d’écran-2022-11-18-154631.png "Configuration YAML")

Il possède un éditeur Rich text et un éditeur markdown pour certain champs.
L'upload des images est facilitée par l'éditeur Rich Text.

![Edition d'un article](img/capture-d’écran-2022-11-18-154802.png "Edition d'un article")

A chaque édition d'un contenu, un commit est envoyé sur le repo précisé dans la configuration (Avec une autorisation de l'app via OAuth pour l'accès au repo GitHub)

# Contre ?

Options de back end limitées à l'utilisation des markdowns. Pas de contenu dynamique
Doit être lié à un système de VCS hébergé (GitHub, GitLab, BitBucket...)