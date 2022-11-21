---
title: Hugo
tags:
  - Hugo
thumbnail: https://www.plemaire.net/img/hugo-featured.png
---
Hugo est un framework qui sert de générateur de site web statique basé sur le markdown

# Pour ? 
Il se base sur des fichiers markdowns pour générer des pages statiques => Léger et peut être transposé facilement à un autre générateur de site statique.
Les fichiers peuvent ne pas être générés par [Netlify CMS](/articles/netlify-cms), tant qu'ils ont les infos nécessaires au bon format.

Assez facile de mettre en place un template custom (cf [Repo GitHub](https://github.com/Pierre-Guichard/victor-hugo)). Il y a un systeme de layout qui est repris pour chaque type de page, personnalisable si nécessaire. Des thèmes sont disponibles, comme pour wordpress.

Les shortcodes sont supportés.

Rapide à compiler, bien intégré avec [Netlify](/articles/netlify). Peut être utilisé sur docker, ou en local (avec la [CLI](https://gohugo.io/installation/))
# Contre ?
Si on veut rajouter un champ dans les fichiers markdowns, il faudra modifier les templates pour qu'ils soient pris en compte.

Nécessite la [CLI](https://gohugo.io/installation/) pour le dev en local. Nécessite [Go](https://go.dev/) (C'est un problème pour les installations docker dans lesquelles il faudra prévoir une image avec Go, au moins jusqu'à la fin de l'étape de build.