---
title: Faut il utiliser Docker ?
tags:
  - Netlify
  - Hugo
  - Netlify CMS
thumbnail: https://www.docker.com/wp-content/uploads/2022/03/Moby-logo.png
---
[Netlify](/articles/netlify) serait remplacé par Docker, pour permettre de déployer ailleurs les fichiers.

[Hugo](/articles/hugo) peut être déployé dans un container Docker
- Pour un environnement de développement, il est possible d'utiliser Docker, même s'il n'est pas forcément nécessaire. La [CLI d'Hugo](https://gohugo.io/commands/) facilite le travail en local sans Docker.
- Pour un environnement de production, on peut utiliser docker, il faudra prévoir un reverse proxy. Cependant, on perd l'intégration continue fournie par [Netlify](/articles/netlify). Il faudrait mettre en place un système de CI/CD qui compenserait cette perte, si le contenu est amené à changer souvent, ou si le client final doit avoir la main sur la publication de ses contenus facilement.

[Netlify Cms](/articles/netlify-cms) est fourni par un CDN appelé depuis l'une des pages statiques. Il n'est donc pas impacté par le container Docker