# Cocon Lacté — site vitrine

Site vitrine réalisé pour Cocon Lacté, l'activité d'accompagnement à l'allaitement et au post-partum d'une amie (facilitatrice d'allaitement, approche Apasdemoa, micro-entreprise individuelle basée dans les Pays de la Loire / Bretagne, en présentiel et en visio).

Projet personnel réalisé en autodidacte, dans le cadre d'une reconversion vers le développement web (avant l'entrée en formation Concepteur Développeur Full Stack). Un vrai besoin, une vraie destinataire : l'occasion de travailler un cahier des charges concret plutôt qu'un exercice fictif.

<!-- Captures d'écran à ajouter ici une fois le contenu finalisé : une vue desktop, une vue mobile. -->

## Voir le site

- En ligne : 
## Stack technique

HTML5 / CSS3 en vanilla, sans framework ni préprocesseur. Un peu de JavaScript prévu pour la suite (menu, formulaire de contact) mais pas encore nécessaire à ce stade.

## Choix techniques et de design

- **Palette de couleurs** extraite du logo, vérifiée avec la formule de contraste WCAG (ratio de luminance) plutôt qu'à l'œil : texte courant à 4,62:1, titres à ~3,15:1 (conforme AA pour du texte large).
- **Variables CSS** (`:root` / `var()`) nommées par rôle (`--couleur-titre`, `--couleur-paragraphe`...) plutôt que par valeur, pour pouvoir ajuster la palette sans réécrire les règles.
- **Typographie** : Dancing Script pour les titres (ambiance douce, manuscrite, cohérente avec la demande de la cliente), Quicksand pour le texte courant, chargées via Google Fonts. Tailles en `rem` pour respecter les préférences d'affichage du navigateur.
- **Mise en page en Flexbox** : menu centré, bandeau décoratif avec navigation imbriquée, section "Qui suis-je ?" en deux colonnes (photo + texte).
- **Bandeau décoratif en forme de nuage** : SVG dessiné à la main (courbes de Bézier), aux couleurs de la marque, plutôt qu'une image bitmap.
- **Responsive** : testé à 375px (mobile) et 768px (tablette). Un correctif `@media` a été nécessaire pour empêcher l'image de la section "Qui suis-je ?" de déborder sur petit écran (comportement des éléments remplacés comme `<img>` en Flexbox).
- **Accessibilité de base** : texte alternatif sur les images, structure sémantique (`header`/`nav`/`main`/`section`/`footer`), contraste vérifié plutôt que supposé.

## État d'avancement

Le site est fonctionnel mais pas terminé. Ce qui reste à faire :

- Textes définitifs des sections Services et Contact
- Section "catalogue de professionnels partenaires" — en attente de confirmation du consentement de chaque personne citée avant publication
- Section tarifs et carte cadeau
- Espacement entre les sections (finitions de mise en page)
- Intégration du logo dans le HTML 
- Interactivité JavaScript légère (menu, formulaire de contact)
- Déploiement sur GitHub Pages

## Structure du projet

```
index.html          — structure de la page (une seule page, sections ancrées)
style.css            — mise en page et palette
script.js             — réservé pour l'interactivité à venir
images/               — logo, photo, bandeau décoratif SVG
```

## Contexte

Ce projet fait partie d'un ensemble de travaux réalisés pendant ma reconversion vers le développement web. Maintenance et mises à jour assurées par moi-même, pas par la cliente.

Développé avec l'assistance de Claude (Anthropic), utilisé comme outil d'apprentissage guidé — explications de concepts, questions pour m'orienter vers la solution, correctifs directs uniquement en cas de bug bloquant (ex. le comportement d'une image en Flexbox sur mobile, documenté ci-dessus) — plutôt que comme générateur de code. Les décisions de design et le code ont été écrits par moi.
