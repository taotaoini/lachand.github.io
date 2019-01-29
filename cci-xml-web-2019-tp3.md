---
layout: default
title: CCI XML et Web 2019
permalink: /teaching/2019/cci-xml-web-2019-tp3
---

# Rendez dynamique votre CV
A partir de ce que vous avez réalisé lors du TP précédent, améliorez votre site pour le rendre plus dynamique

## Creez un fichier javascript
Vous devez maintenant créer un fichier javascript script-cv.js et devez l'intégrer dans votre fichier HTML.
Rappel : pour inclure un fichier javascript dans notre page HTML, nous devons utiliser la commande suivante dans le **<head>...</head>** de notre document
``` html
<script type = "text/javascript" src = "filename.js" ></script>
```

## Ajoutez une barre de progression à votre site
Pour que l'utilisateur sache quelle est sa progression sur votre CV, vous allez rajouter un barre de progression en haut de votre site.

Regardez la documentation sur le site de material design lite (https://getmdl.io/components/index.html#sliders-section)[https://getmdl.io/components/index.html#sliders-section] pour voir comment configurer le slider.

Votre barre de progression doit avoir l'id suivant : **progress_bar**

Afin que votre slider soit toujours visible, fixez l'élément (https://j-willette.developpez.com/tutoriels/css/position-fixed/)[https://j-willette.developpez.com/tutoriels/css/position-fixed/]

## Faites le lien entre scroll et barre de progression
Vous allez maintenant lier la barre de progression et le scroll de l'utilisateur. Afin de récupérer l'évènement quand l'utilisateur scroll sur la page et afin de calculer le pourcentage de page visité, aidez vous du lien suivant : (https://www.w3schools.com/jsref/event_onscroll.asp)[https://www.w3schools.com/jsref/event_onscroll.asp]

Vous devez calculer la valeur en pourcentage du scroll.

En vous aidant de la documentation de material design lite, modifiez la valeur de la barre de progression en fonction du scroll de l'utilisateur.

## Faites le lien entre la barre de progression et le scroll
Vous allez maintenant permettre à l'utilisateur de descendre et monter dans votre page à l'aide de la barre de progression.

En ajoutant l'attribut onChange (https://www.w3schools.com/jsref/event_onchange.asp)[https://www.w3schools.com/jsref/event_onchange.asp] à votre barre de progression, faites appel à une fonction que vous définissez dans votre fichier javascript pour naviguer dans la page.
Pour ceci, vous aller récupérer la valeur en pourcentage de la barre de progression à l'aide du code suivant :
```javascript
var progress = document.getElementById('progress_bar').value; // valeur de la barre de progression
```
