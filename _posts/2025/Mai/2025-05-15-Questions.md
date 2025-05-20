---
layout: post
title:  "Questions / Réponses"
date:   2025-05-14 08:00
categories: .NET C#
---
## Incoma/Tremplin
### Couches
- FE: 
  - structure npm ? Webpack
  - blocks: incoma commun aux mesures
  - pas blocks: propre à la mesure
  - les pages webs utilisent principalement des webcompos
  - le js appelle un script js nommé xxx-services.js
  - ce script de service appele via des api, des controlers.
  - Ces contrôleurs appellent le backend à l'aide de clients créés.
  - Si un contrôleur déclanche une transition historique, un message ASB est lancé, alors le code sera intercepté côté BE par l'orchestrateur et cherchera les Handler a déclencher qui ont ce code setté en propriété.
- BE: 
  - 