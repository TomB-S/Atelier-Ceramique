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

- Fraunces (titres) — serif organique, plus texturée et chaleureuse
- Work Sans (corps de texte) — lisibilité et modernité

**Formes**

- Blobs (border-radius asymétrique) en fond du hero et en motif décoratif récurrent
- Aplats de couleur francs sur les cartes "valeurs" et le bloc CTA plutôt que des fonds pastel discrets
- Coins très arrondis sur cartes et boutons (CTA en forme de pilule)

## Choix techniques

**Bootstrap 5.3.3** via CDN pour la grille responsive, le système de colonnes et le composant navbar avec burger menu mobile

**CSS Custom** pour la charte graphique, les variables CSS (couleurs, radius, ombres, dégradés), le hero à blobs, l'effet hover sur la galerie et le responsive mobile-first

**Bootstrap Icons** pour les icônes des valeurs et les réseaux sociaux du footer

**Google Fonts** via CDN pour les polices Fraunces et Work Sans

## Structure de la mise en page

- Header : navbar Bootstrap `navbar-expand-md` — burger menu sous 768px, liens horizontaux au-dessus
- Hero : fond brun foncé avec blobs terracotta/ocre/vert olive en pseudo-éléments `::before`/`::after`, texte avec `text-shadow` pour rester lisible au-dessus des blobs
- Grilles : Bootstrap `col-md-*` pour les sections à propos (6/6), valeurs (4/4/4), sélection (3/3/3/3) et galerie (4/4/4)
- Footer : flexbox colonne sur mobile, ligne sur tablette et desktop via media queries
- Responsive : approche mobile-first avec breakpoints à 768px et 1200px

## À venir

Points d'ancrage déjà posés dans le HTML pour une prochaine phase de comportements JavaScript (non implémentée) :

- `data-lightbox="galerie"` sur les images de `galerie.html` — pour une visionneuse plein écran
- classe `.reveal` sur les sections principales des 3 pages — pour des animations au scroll
- validation HTML5 native du formulaire de contact, à enrichir en JS (retour temps réel)
