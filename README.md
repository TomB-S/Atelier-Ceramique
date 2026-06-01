# Atelier Céramique Lyon

Site vitrine 3 pages pour un atelier de céramique artisanale lyonnais.

## Pages

**index.html** : Accueil avec hero pleine largeur, section à propos, valeurs, sélection d'œuvres et CTA contact
**galerie.html** : Galerie d'œuvres en grille responsive avec effet zoom et overlay au survol
**contact.html** : Formulaire de contact avec validation HTML5 native et infos pratiques (carte Google Maps)

## Charte graphique

**Couleurs**

- Terracotta `#c0673a` — header, boutons principaux
- Ocre `#d4a055` — sections alternées, cards valeurs
- Vert olive `#6b7c4b` — hover, détails
- Brun foncé `#2c1810` — texte principal, footer
- Crème `#faf3ec` — fond général de la page

**Typographie**

- Playfair Display (titres) — caractère artisanal et élégant
- Lato (corps de texte) — lisibilité et modernité

## Choix techniques

**Bootstrap 5.3.3** via CDN pour la grille responsive, le système de colonnes et le composant navbar avec burger menu mobile

**CSS Custom** pour la charte graphique, les variables CSS, le hero avec overlay, l'effet hover sur la galerie et le responsive mobile-first

**Bootstrap Icons** pour les icônes des valeurs et les réseaux sociaux du footer

**Google Fonts** via CDN pour les polices Playfair Display et Lato

## Structure de la mise en page

- Header : navbar Bootstrap `navbar-expand-md` — burger menu sous 768px, liens horizontaux au-dessus
- Hero : image pleine largeur avec pseudo-élément `::before` pour l'overlay sombre
- Grilles : Bootstrap `col-md-*` pour les sections à propos (6/6), valeurs (4/4/4), sélection (3/3/3/3) et galerie (4/4/4)
- Footer : flexbox colonne sur mobile, ligne sur tablette et desktop via media queries
- Responsive : approche mobile-first avec breakpoints à 768px et 1200px
