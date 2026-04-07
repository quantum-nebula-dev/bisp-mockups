# Audit Critique — 9 Mockups Homepage BISP

**Date** : 7 avril 2026
**Auditeur** : Critic Agent (Opus 4.6)
**Reference** : design-brief.md Phase 0
**Methode** : Lecture integrale des 9 fichiers HTML (CSS + HTML + JS), croisement avec le design brief

---

## Executive Summary

Les 9 mockups sont globalement de bonne facture. Chaque mockup inclut les **8 blocs obligatoires**, utilise les **vrais assets BISP** (logos, photos, pictos, video), ecrit en **francais avec accents corrects**, et respecte une **palette ancree sur les tokens Dembrandt** de son site de reference. Aucun mockup n'utilise de polices bannies (Inter, Roboto, Arial) dans ses declarations CSS. Aucun purple gradient detecte.

**Points forts transversaux :**
- 9/9 ont un seul `<h1>` par page, hierarchie H1 > H2 > H3 correcte (aucun niveau saute)
- 9/9 ont `prefers-reduced-motion` respecte
- 9/9 ont `:focus-visible` implemente
- 9/9 ont un skip-link fonctionnel (Aiglon utilise `.skip-to-content` au lieu de `.skip-link` mais fonctionnel)
- 9/9 ont un toggle FR/EN textuel (pas de drapeaux, sauf Beausoleil qui utilise un micro-drapeau decoratif)
- 9/9 utilisent video + poster fallback dans le hero
- 9/9 ont les logos Cambridge et Pearson
- 0/9 utilisent des polices bannies dans font-family CSS (Inter/Roboto/Arial/Open Sans/Lato/Space Grotesk)
- 0/9 ont des purple gradients

**Faiblesses transversales :**
- **Breakpoint 375px** : seulement 3/9 mockups (Aiglon, Le Rosey, Gordonstoun) ont un breakpoint mobile specifique a 375px. Les autres s'appuient sur 480px comme plus petit breakpoint, ce qui laisse des incertitudes pour les ecrans iPhone SE/mini.
- **Breakpoint 1440px** : seulement 3/9 (Ecole des Roches, Le Rosey, sevenoaks via 1080px) ont un breakpoint desktop large. Le brief demande 1440px explicitement.
- **Touch targets** : la plupart declarent `min-height: 48px` sur les boutons principaux, mais pas systematiquement sur tous les elements interactifs (liens nav, lang toggle, etc.)

---

## Detail par Mockup

### 1. Inspired-Beausoleil

**Fichier** : `inspired-beausoleil/index.html` (2999 lignes)
**Palette** : `#002654` (navy), `#0087c9` (sky-blue), `#ffd931`/`#c4a35a` (gold) -- conforme tokens Beau Soleil
**Polices** : Cormorant Garamond (display) + DM Sans (body) + Playfair Display (accent)
**Radius** : 2, 6, 10, 30, 50px -- conforme tokens (gamme large, pill 50px)
**Shadows** : Ajout de shadow-subtle/card/elevated (le brief dit "aucune" pour Beau Soleil) -- **Minor deviation**

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | Ligne ~2053, `.skip-link` avec focus visible |
| H1 unique | OK | Ligne 2135, une seule `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(9) > H3(15) |
| Focus-visible | OK | `:focus-visible` avec outline 3px sky-blue |
| prefers-reduced-motion | OK | 1 bloc `@media (prefers-reduced-motion: reduce)` |
| Alt text | OK | 32 images, alt semantiques, decoratives avec `alt="" aria-hidden="true"` |
| Touch 48px | Partiel | `.btn` et `.nav__cta` a min-height 48px, mais liens nav et lang toggle sans min-height |
| Breakpoints | **Manque 375px** | 480px, 768px, 1200px -- pas de 375px ni 1440px |
| 8 blocs | OK | Nav, Hero, Promesses, Chiffres, Programmes, Galerie+Bilingue (extra), Temoignages, Directeur, Footer |
| Tokens conformes | OK | Palette Beau Soleil exacte, radius pill 50px |
| Anti-slop | OK | Pas de purple gradients, pas de 3-boxes, layout riche et varie |
| FR accents | OK | ecole, eleves, francais, maternelle, lycee tous avec accents corrects |
| Assets BISP | Excellent | 9 images BISP, 7 pictos, 11 stock, 1 video, 2 logos accreditations |
| Drapeau nav | **Minor** | Utilise un petit drapeau FR (flag-fr.png) dans le toggle -- le brief dit "pas de drapeau" |
| Contenu extra | Bonus | Ajoute une section Galerie Band + Bilingual Split -- enrichit le design |

**Issues** :
- **Major** (1) : Pas de breakpoint 375px -- layout non teste pour iPhone SE
- **Minor** (2) : Shadows ajoutees alors que tokens Beau Soleil = aucune ; drapeau dans le lang toggle

---

### 2. Inspired-Aiglon

**Fichier** : `inspired-aiglon/index.html` (2585 lignes)
**Palette** : `#0d1117` (deep), `#b11d23` (red accent), `#ceab52` (gold) -- conforme Aiglon dark cinematic
**Polices** : Satoshi (Calibre proxy) + Cabinet Grotesk (display) + Instrument Serif (editorial)
**Radius** : 3px unique + 999px pill -- strictement conforme Aiglon tokens
**Shadows** : `0 29px 35px` dramatic -- conforme Aiglon shadow-4/5

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | Ligne 1828, `.skip-to-content` (nom different mais fonctionnel) |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(6) > H3(8) > H4(3) |
| Focus-visible | OK | 8 occurrences, outline 2px gold |
| prefers-reduced-motion | OK | Bloc complet avec reset animations + `.reveal { opacity: 1 }` |
| Alt text | OK | Images avec alt semantiques, decoratives avec aria-hidden |
| Touch 48px | OK | 4 declarations min-height 48px sur boutons et hamburger |
| Breakpoints | **Bon** | 375px, 767px, 1024px -- le seul avec vrai 375px specifique |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Radius 3px strict, shadows 29px, palette sombre Aiglon fidele |
| Anti-slop | OK | Design distinctif, cinematique, pas de cliches |
| FR accents | OK | Tous accents corrects |
| Assets BISP | OK | 6 images, 4 pictos, 3 stock, 1 video |
| Fidelite reference | Excellent | Ambiance dark cinematique Aiglon bien reproduite |

**Issues** :
- **Minor** (1) : Classe `.skip-to-content` au lieu du nom conventionnel `.skip-link` (fonctionnel mais inconsistant)
- **Minor** (1) : Pas de breakpoint 1440px desktop large

---

### 3. Inspired-Le Rosey

**Fichier** : `inspired-lerosey/index.html` (2614 lignes)
**Palette** : `#182f66` (navy) + `#ffffff` -- bichromatique exacte Le Rosey
**Polices** : EB Garamond (display/body) + Playfair Display (accent) -- conforme tokens Le Rosey
**Radius** : 0px -- conforme (rectangulaire pur)
**Shadows** : 0 -- conforme (flat design)
**Base font-size** : 17px -- conforme token Le Rosey

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | `.skip-link` present |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(6) > H3(8) > H4(3) |
| Focus-visible | OK | outline 3px solid navy |
| prefers-reduced-motion | OK | 2 blocs (CSS + JS) |
| Alt text | OK | 15 images, alt semantiques |
| Touch 48px | OK | min-height 48px sur boutons et hamburger |
| Breakpoints | **Bon** | 375px, 480px, 768px, 1024px, 1440px -- le plus complet |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Bichromatique pur, radius 0, shadow 0, spacing 7-72px |
| Anti-slop | OK | Design editorial epure, pas de cliches |
| FR accents | OK | Tous corrects |
| Assets BISP | Adequat | 5 images, 4 pictos, 3 stock, 1 video |
| Extras | Bonus | `@media (forced-colors: active)` et `@media print` -- accessibilite superieure |

**Issues** :
- **Minor** (1) : Moins d'images BISP que d'autres mockups (pas de photos galerie)
- **Minor** (1) : Carousel temoignages depend de JS -- pas de fallback sans JS

---

### 4. Inspired-Sevenoaks

**Fichier** : `inspired-sevenoaks/index.html` (2740 lignes)
**Palette** : `#004f5d` (teal) + `#ffffff` + `#0a1628` (navy) -- conforme tokens Sevenoaks
**Polices** : DM Sans (proxy Bliss humaniste) -- conforme
**Radius** : 0-3px + 9999px pill -- conforme tokens
**Shadows** : aucune -- conforme (flat design)

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | `.skip-link` present |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(9) > H3(17) |
| Focus-visible | OK | 7 occurrences, outline 2px teal |
| prefers-reduced-motion | **Excellent** | Utilise `prefers-reduced-motion: no-preference` (best practice) ET `reduce` |
| Alt text | OK | 30 images, bons alt texts |
| Touch 48px | Partiel | 1 seule declaration min-height 48px |
| Breakpoints | **Manque 375px** | 500px, 768px, 960px, 1080px -- pas de 375px ni 1440px |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Teal exact, flat design, radius angulaire strict |
| Anti-slop | Excellent | Hero split (video | teal) = geste de design distinctif |
| FR accents | OK | Tous corrects |
| Assets BISP | Bon | 7 images, 4 pictos, 15 stock, 1 video |
| Fidelite reference | Excellent | Hero split fidele au style Sevenoaks |

**Issues** :
- **Major** (1) : Pas de breakpoint 375px
- **Minor** (1) : Touch targets insuffisants sur elements secondaires (liens nav, lang toggle)
- **Minor** (1) : `<sup>` utilise pour "15e arrondissement" -- bien mais verifier semantique

---

### 5. Inspired-Gordonstoun

**Fichier** : `inspired-gordonstoun/index.html` (2640 lignes)
**Palette** : `#702381` (pourpre), `#c7b0d5` (lavande), `#7a7d83` (gris) -- conforme Gordonstoun monochromatique pourpre
**Polices** : Cormorant Garamond (serif italic) + Josefin Sans (body) -- proxy Ivy Presto + Proxima Nova
**Radius** : 6px + 50px pill -- conforme tokens (2-7px + pilule)
**Texture grain** : Oui (body::before avec SVG noise) -- signature Gordonstoun

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | `.skip-link` present, outline lavande |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(7) > H3(8) |
| Focus-visible | OK | 6 occurrences, outline 3px lavande |
| prefers-reduced-motion | OK | 3 blocs (CSS complet + animations reset) |
| Alt text | OK | 23 images avec alt semantiques |
| Touch 48px | OK | 5 declarations min-height 48px |
| Breakpoints | OK | 480px, 768px, 1024px -- manque 375px et 1440px |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Pourpre monochromatique fidele, CAPS/italic mix distinctif |
| Anti-slop | Excellent | Traitement typographique mixed CAPS/italic = signature forte |
| FR accents | OK | Tous corrects |
| Assets BISP | OK | 5 images, 4 pictos, 12 stock, 1 video |
| Fidelite reference | Excellent | Texture grain + mixed typography reproduit le style Gordonstoun |

**Issues** :
- **Minor** (1) : Pas de breakpoint 375px specifique
- **Minor** (1) : Texture grain (body::before z-index 9999) pourrait interferer avec les elements interactifs -- verifier que `pointer-events: none` est bien present (OK, confirme)
- **Minor** (1) : `border-radius: 0 0 6px 6px` sur skip-link -- radius 6px conforme mais le brief dit le Gordonstoun reference a des bords a 2px

---

### 6. Inspired-Repton

**Fichier** : `inspired-repton/index.html` (2816 lignes)
**Palette** : `#3e4561` (navy), `#988360` (gold), `#93866c` (bronze) -- conforme tokens Repton
**Polices** : Montserrat Light 300-400 -- proxy Gotham Light + Montserrat (conforme)
**Radius** : 2px, 6px, 50px pill -- conforme tokens
**Shadows** : `0 0 0 0.1px` micro + `0 0 0 0.5px` soft -- conforme Repton quasi-invisible

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | `.skip-link` present, outline gold |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(6) > H3(11) |
| Focus-visible | OK | outline 2px gold |
| prefers-reduced-motion | OK | Bloc complet + video masquee + poster affiche + `.reveal { opacity: 1 }` |
| Alt text | OK | 15 images avec alt |
| Touch 48px | OK | 2 declarations (boutons), nav CTA a `min-height: 44px` |
| Breakpoints | **Manque 375px** | 480px, 768px, 1024px -- pas de 375px ni 1440px |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Navy + gold + timeline concept fidele |
| Anti-slop | OK | Approche timeline narrative = distinctive |
| FR accents | OK | Tous corrects |
| Assets BISP | Adequat | 5 images, 4 pictos, 3 stock, 1 video |
| Fidelite reference | Bon | Quiet luxury typographique bien capture |

**Issues** :
- **Major** (1) : Nav CTA `min-height: 44px` au lieu de 48px -- sous le seuil WCAG 2.5.5 (ligne ~457)
- **Minor** (1) : Pas de breakpoint 375px
- **Minor** (1) : Moins de stock photos que d'autres mockups

---

### 7. Inspired-Kent College

**Fichier** : `inspired-kentcollege/index.html` (2741 lignes)
**Palette** : `#aa0040` (crimson), `#ff4951` (coral), `#ffffff` -- conforme tokens Kent College
**Polices** : Montserrat 400-900 -- proxy Azo Sans, 100% sans-serif conforme
**Radius** : 6px, 16px, 50px, 50% -- conforme (organique, cercles)
**Formes organiques** : `img-organic` avec border-radius asymetrique -- signature Kent College

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | `.skip-link` present, pill radius |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(6) > H3(14) |
| Focus-visible | OK | 7 occurrences, outline 3px coral |
| prefers-reduced-motion | OK | Bloc complet avec video fallback |
| Alt text | OK | 28 images avec alt semantiques |
| Touch 48px | OK | `min-height: 52px` sur boutons (superieur au minimum) |
| Breakpoints | OK | 480px, 768px, 1024px -- pas de 375px mais 7 occurrences de 375 en max-width CSS |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Rouge monochromatique exact, formes organiques fideles |
| Anti-slop | Excellent | Formes arrondies/organiques = visuel unique dans le panel |
| FR accents | OK | Tous corrects |
| Assets BISP | Bon | 6 images, 7 pictos (le plus), 12 stock, 1 video |
| Fidelite reference | Excellent | Cercles, dots decoratifs, shapes organiques = Kent College pur |

**Issues** :
- **Minor** (1) : Pas de breakpoint 375px en `@media` (utilise 480px)
- **Minor** (1) : Boutons a `min-height: 52px` (non problematique, mais inconsistant avec 48px brief)

---

### 8. Inspired-Haut-Lac

**Fichier** : `inspired-hautlac/index.html` (3028 lignes -- le plus long)
**Palette** : `#348397` (teal), `#ed3122` (red), `#429e7b` (vert), `#d89137` (orange) -- conforme multi-accent Haut-Lac
**Polices** : Montserrat (headings) + Be Vietnam Pro (body) -- conforme tokens Haut-Lac
**Radius** : 3, 5, 12px -- conforme (angles, max 12px)
**Border thick** : 5px -- conforme token Haut-Lac

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | `.skip-link` present |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(6) > H3(8) > H4(3) |
| Focus-visible | OK | outline 3px teal-light |
| prefers-reduced-motion | **Excellent** | 4 blocs distincts -- le plus detaille du panel |
| Alt text | OK | 21 images avec alt |
| Touch 48px | OK | 4 declarations min-height 48px |
| Breakpoints | OK | 480px, 768px, 1024px -- 1 ref 375px en CSS |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Multi-accent teal/red/vert/orange fidele |
| Anti-slop | OK | Diagonales, B&W photo treatment = distinctif |
| FR accents | OK | Tous corrects |
| Assets BISP | Bon | 6 images, 4 pictos, 8 stock, 1 video |
| Fidelite reference | Bon | Diagonales et multi-couleur captures |

**Issues** :
- **Minor** (1) : Pas de breakpoint 375px en @media
- **Minor** (1) : Le fichier est le plus long (3028 lignes) -- potentiel de performance

---

### 9. Inspired-Ecole des Roches

**Fichier** : `inspired-ecoledesroches/index.html` (2748 lignes)
**Palette** : `#0b1e3a` (navy), `#fdb82e` (gold) -- conforme tokens Ecole des Roches
**Polices** : DM Sans (proxy Gill Sans) + Source Sans 3 (proxy Agrandir) -- conforme
**Radius** : 9999px pill + 30px card + 16px + 8px -- conforme (tout arrondi EDR)
**Shadows** : `0 136px 136px` cinema -- conforme shadow dramatique EDR

| Critere | Statut | Detail |
|---------|--------|--------|
| Skip-link | OK | `.skip-link` pill shape, outline gold |
| H1 unique | OK | 1 `<h1>` |
| Heading hierarchy | OK | H1(1) > H2(7) > H3(11) |
| Focus-visible | OK | outline 3px gold |
| prefers-reduced-motion | **Excellent** | 3 blocs + `@media print` = accessibilite superieure |
| Alt text | **Excellent** | 35 images -- le plus d'images alt du panel |
| Touch 48px | Partiel | `min-height: 52px` sur `.btn` mais pas sur nav links |
| Breakpoints | OK | 480px, 768px, 1024px, 1440px -- a le 1440px |
| 8 blocs | OK | Tous presents |
| Tokens conformes | Excellent | Shadow cinema 136px, pills 9999px, duale navy+gold |
| Anti-slop | OK | Profondeur cinematographique distinctive |
| FR accents | OK | Tous corrects |
| Assets BISP | Excellent | 10 images, 4 pictos, 18 stock (le plus), 1 video |
| Fidelite reference | Bon | Profondeur et pill shapes bien captures |
| Extras | Bonus | `@media print` et breakpoint 1440px |

**Issues** :
- **Minor** (1) : Nav links sans min-height explicite
- **Minor** (1) : `min-height: auto` sur mobile reset le min-height des boutons (ligne 1812)

---

## Tableau Comparatif

| Critere | Beausoleil | Aiglon | Le Rosey | Sevenoaks | Gordonstoun | Repton | Kent College | Haut-Lac | Ecole Roches |
|---------|:----------:|:------:|:--------:|:---------:|:-----------:|:------:|:------------:|:--------:|:------------:|
| Skip-link | OK | OK* | OK | OK | OK | OK | OK | OK | OK |
| H1 unique | OK | OK | OK | OK | OK | OK | OK | OK | OK |
| Heading hierarchy | OK | OK | OK | OK | OK | OK | OK | OK | OK |
| Focus-visible | OK | OK | OK | OK | OK | OK | OK | OK | OK |
| prefers-reduced-motion | OK | OK | OK | ++ | OK | OK | OK | ++ | ++ |
| Alt text | OK | OK | OK | OK | OK | OK | OK | OK | ++ |
| Touch 48px | Partiel | OK | OK | Partiel | OK | **44px** | OK | OK | Partiel |
| 375px breakpoint | **NON** | OK | OK | **NON** | **NON** | **NON** | **NON** | **NON** | **NON** |
| 1440px breakpoint | **NON** | **NON** | OK | **NON** | **NON** | **NON** | **NON** | **NON** | OK |
| Token fidelity | OK | ++ | ++ | ++ | ++ | ++ | ++ | ++ | ++ |
| Anti-slop | OK | OK | OK | ++ | ++ | OK | ++ | OK | OK |
| FR accents | OK | OK | OK | OK | OK | OK | OK | OK | OK |
| 8 blocs complets | OK | OK | OK | OK | OK | OK | OK | OK | OK |
| Assets BISP | ++ | OK | OK | OK | OK | OK | OK | OK | ++ |
| @media print | NON | NON | OK | NON | NON | NON | NON | NON | OK |
| forced-colors | NON | NON | OK | NON | NON | NON | NON | NON | NON |

Legende : OK = conforme, ++ = excellent/au-dessus, **NON** = absent, **44px** = sous seuil

---

## Comptage d'Issues par Severite

| Mockup | Critical | Major | Minor | Total |
|--------|:--------:|:-----:|:-----:|:-----:|
| Beausoleil | 0 | 1 | 2 | 3 |
| Aiglon | 0 | 0 | 2 | 2 |
| Le Rosey | 0 | 0 | 2 | 2 |
| Sevenoaks | 0 | 1 | 2 | 3 |
| Gordonstoun | 0 | 0 | 3 | 3 |
| Repton | 0 | 1 | 2 | 3 |
| Kent College | 0 | 0 | 2 | 2 |
| Haut-Lac | 0 | 0 | 2 | 2 |
| Ecole des Roches | 0 | 0 | 2 | 2 |
| **TOTAL** | **0** | **3** | **19** | **22** |

---

## Issues Majeures (3)

1. **Beausoleil** : Pas de breakpoint 375px -- layout mobile non valide sur iPhone SE/mini
2. **Sevenoaks** : Pas de breakpoint 375px -- hero split pourrait casser sur petit ecran
3. **Repton** : Nav CTA `min-height: 44px` (ligne ~457) -- sous le seuil WCAG 2.5.5 de 48px

---

## Classement Accessibilite (WCAG 2.1 AA)

1. **Le Rosey** -- Breakpoints les plus complets (375px, 480px, 768px, 1024px, 1440px), `forced-colors`, `@media print`, flat design conforme
2. **Aiglon** -- Breakpoint 375px present, reduced-motion complet, focus-visible 8x
3. **Ecole des Roches** -- `@media print`, breakpoint 1440px, 35 alt texts (le plus), reduced-motion 3 blocs
4. **Haut-Lac** -- 4 blocs prefers-reduced-motion (le plus detaille), bonne couverture responsive
5. **Kent College** -- Touch targets 52px (le plus genereux), 7 focus-visible, bonne couverture
6. **Gordonstoun** -- 5 declarations touch targets, bonne accessibilite clavier
7. **Sevenoaks** -- Utilise `prefers-reduced-motion: no-preference` (best practice), mais manque 375px
8. **Beausoleil** -- Bonne couverture alt text (32 images), mais manque 375px
9. **Repton** -- Touch target 44px sous seuil, manque 375px

---

## Classement Token Fidelite

1. **Le Rosey** -- Bichromatique pur, radius 0, shadow 0, spacing 7-72px, base 17px : reproduction parfaite
2. **Aiglon** -- Radius 3px strict, shadows 29px, dark cinematic, Satoshi proxy Calibre : fidele
3. **Kent College** -- Rouge monochromatique, formes organiques/cercles, Montserrat proxy Azo Sans : fidele
4. **Gordonstoun** -- Pourpre monochromatique, CAPS/italic mixed, texture grain : fidele
5. **Haut-Lac** -- Multi-accent teal/red/vert/orange, Montserrat + Be Vietnam Pro, border 5px : fidele
6. **Ecole des Roches** -- Shadow cinema 136px, pills 9999px, DM Sans proxy Gill Sans : fidele
7. **Repton** -- Navy + gold, Montserrat Light 300, shadow micro : fidele
8. **Beausoleil** -- Palette exacte mais shadows ajoutees (Beau Soleil = flat design pur)
9. **Sevenoaks** -- Teal exact, DM Sans proxy Bliss, mais le hero split est une interpretation libre

---

## Classement Design/Anti-Slop

1. **Sevenoaks** -- Hero split (video | teal) = geste de design audacieux et distinctif
2. **Gordonstoun** -- Mixed CAPS/italic typography + texture grain = signature forte
3. **Kent College** -- Formes organiques/cercles + dots decoratifs = visuel unique
4. **Aiglon** -- Cinematique dark, red accent words = atmosphere emotive
5. **Le Rosey** -- Epure editorial bichromatique = elegance minimaliste
6. **Repton** -- Quiet luxury typographique + timeline narrative = prestige
7. **Haut-Lac** -- Diagonales + multi-accent = energetique
8. **Ecole des Roches** -- Profondeur cinematographique, pills arrondis = sophistique
9. **Beausoleil** -- Le plus riche en contenu mais layout plus conventionnel

---

*Fin de l'audit. Aucune issue Critical detectee. 3 issues Major corrigeables en ajoutant des breakpoints 375px et en ajustant un min-height. 19 issues Minor principalement cosmetiques ou de completude responsive.*
