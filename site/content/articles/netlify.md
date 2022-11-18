---
title: Netlify
tags:
  - Netlify
---
Netlify est une plateforme qui permet le déploiement automatique et rapide de sites statiques.

C'est un SASS.

# Principe

A chaque commit sur la branche précisée dans la configuration, le code est mis à jour : L'appli est build à nouveau, le site statique est mis à jour.

![Liste des build en fonction des commits](img/capture-d’écran-2022-11-18-151746.png "Liste des build en fonction des commits")

Les sites utilisant Netlify CMS ne sont pas forcément déployées sur Netlify. Les sites sur Netlify n'utilisent pas forcément netlifyCMS.

# Technos

On peut choisir les technologies qui sont les plus adaptées au projet en cours. Dans le cas d'un site comme [EIG ](https://eig.etalab.gouv.fr/), on a :
- [Netlify CMS](/articles/netlify-cms), qui génère les fichiers markdown depuis son interface et créé des commits
- [Hugo](/articles/hugo) ( avec le template [Victor Hugo](https://github.com/netlify-templates/victor-hugo) ) qui interprète les fichiers markdown et les rends en fichiers statiques.

# Déploiement
## Docker ?
L'utilisation de Docker est possible, mais elle vient remplacer Netlify. On perd l'automatisation de la build en fonction des commits. Il faudrait mettre en place un système de CI/CD pour automatiser les mises à jours et retrouver le principe de Netlify qui mets cela à disposition rapidement
## Environnement de dev 
RAS : Les caractéristiques sont liées à l'utilisateur du framework front

