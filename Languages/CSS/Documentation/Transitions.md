# Transitions

https://developer.mozilla.org/fr/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions
https://developer.mozilla.org/fr/docs/Web/CSS/transition

Les **transitions CSS** permettent de contrôler la vitesse d'animation lorsque les propriétés CSS sont modifiées. Plutôt que le changement soit immédiat, on peut l'étaler sur une certaine période. Ainsi, si on souhaite passer un élément de blanc à noir, on pourra utiliser les transitions CSS afin que cette modification soit effectuée progressivement, selon une courbe d'accélération donnée.

Les animations qui utilisent des transitions entre deux états sont souvent appelées _transitions implicites_ car l'état initial et l'état final sont définis implicitement par le navigateur.

Les transitions CSS vous permettent de choisir :
-   les propriétés à animer en les listant explicitement
-   le début de l'animation
-   la durée de l'animation
-   la façon dont la transition s'exécutera


#### Un exemple simple
Avec cette feuille de style, on opère une transition CSS sur la taille de police de quatre secondes après deux secondes écoulées lorsque l'utilisateur passe la souris sur l'élément :
```css
#delay {
  font-size: 14px;
  transition-property: font-size;
  transition-duration: 4s;
  transition-delay: 2s;
}

#delay:hover {
  font-size: 36px;
}
```