# Animations

https://developer.mozilla.org/fr/docs/Web/CSS/CSS_Animations/Using_CSS_animations
https://developer.mozilla.org/fr/docs/Web/CSS/animation

#### Generators
- https://animista.net/play/basic
- https://animate.style/

Les **animations CSS** permettent de créer des transitions entre deux états de mise en forme. Une animation est décrite par deux choses : des propriétés propres à l'animation d'une part et un ensemble d'étapes (_keyframes_) qui indiquent l'état initial, final et éventuellement des états intermédiaires d'autre part.

```css
p {
  animation-duration: 3s;
  animation-name: slidein;
}

@keyframes slidein {
  from {
    margin-left: 100%;
    width: 300%;
  }

  to {
    margin-left: 0%;
    width: 100%;
  }
}

```