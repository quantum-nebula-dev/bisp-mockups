# Scoring Report — 9 Mockups Homepage BISP

**Date** : 7 avril 2026
**Juge** : Judge Agent (Opus 4.6)
**Références** : design-brief.md, handoff-phase1.md, critic-audit.md, 9 screenshots de référence, 9 mockups HTML lus intégralement
**Méthode** : Lecture complète des 9 fichiers HTML (CSS + HTML + JS), comparaison visuelle avec les screenshots des 9 sites de référence, croisement avec le design brief et l'audit du Critic

---

## 1. Executive Summary

### Top 3

| Rang | Mockup | Score global | Verdict |
|------|--------|:------------:|---------|
| **1** | **Inspired-Aiglon** | **84/100** | Design cinématique sombre d'une sophistication rare. Fidélité tokens excellente (radius 3px, shadow 29px, palette dark). Le traitement "mots rouges" dans les titres crée une signature visuelle immédiate. Meilleur équilibre fidélité-originalité-UX du panel. |
| **2** | **Inspired-Le Rosey** | **81/100** | Pureté bichromatique magistrale. Radius 0, shadow 0, spacing 7-72px : reproduction parfaite des tokens. L'élégance éditoriale serif crée une gravitas rare. Breakpoints les plus complets du panel (375-1440px). Accessibilité exemplaire. |
| **3** | **Inspired-Sevenoaks** | **79/100** | Le hero split (vidéo | teal) est le geste de design le plus audacieux et mémorable du panel. DM Sans comme proxy Bliss fonctionne bien. Le flat design teal est distinctif sans être tape-à-l'œil. Pénalisé par l'absence de breakpoint 375px. |

**Score moyen du panel** : 73.4/100
**Mockups au-dessus du seuil (70/100)** : 7/9
**Mockups sous le seuil** : Beau Soleil (68/100), Haut-Lac (67/100)

---

## 2. Scoring détaillé par mockup

### Grille de pondération

| Critère | Poids |
|---------|:-----:|
| Fidélité à la référence | 20% |
| Alignement marque BISP | 20% |
| UX / Conversion | 20% |
| Originalité dans l'adaptation | 20% |
| Anti-slop + Accessibilité | 20% |

---

### 2.1 Inspired-Aiglon — 84/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 9 | 18 | Reproduction exceptionnelle de l'ambiance cinématique Aiglon. Palette dark (#0d1117, #b11d23, #ceab52) exacte. Radius 3px strict conforme. Shadows 29px dramatiques conformes. Satoshi comme proxy Calibre est le meilleur choix de police proxy du panel. Cabinet Grotesk pour les display + Instrument Serif pour l'éditorial créent un trio typographique riche. |
| Alignement BISP | 8 | 16 | 4 piliers présents et bien intégrés. Le ton "confiant" est palpable dans le traitement dramatique. Les mots rouges dans les titres ("langues", "élèves", "monde") créent une hiérarchie émotionnelle. 8 blocs complets. Textes hero conformes. Le traitement sombre est peut-être légèrement intimidant pour le pilier "chaleureux", mais la qualité compense. |
| UX / Conversion | 8 | 16 | Navigation visible et fonctionnelle avec 5 items. Toggle FR/EN textuel segmenté (FR|EN) avec état actif clair. CTA "Planifier une visite" bien visible. Parcours parent logique. Floating CTA mobile. Breakpoint 375px présent. Carrousel témoignages avec prev/next. Escape key ferme le menu mobile. |
| Originalité | 9 | 18 | Le traitement "red accent words" dans les titres est une adaptation créative brillante du style Aiglon (qui utilise des mots rouges dans ses titres). La texture sombre immersive transporte l'ambiance cinématique Aiglon dans le contexte parisien de BISP. Les wave separators SVG entre sections ajoutent du rythme. 6 témoignages diversifiés (franco-allemande, britannique, japonaise, marocain, italienne, américain). |
| Anti-slop + Accessibilité | 8 | 16 | Satoshi + Cabinet Grotesk + Instrument Serif : aucune police bannie. Skip-link fonctionnel. 8 occurrences focus-visible. prefers-reduced-motion complet avec fallback `.reveal { opacity: 1 }`. Pas de breakpoint 1440px (minor). Textes français avec accents. Palette ancrée sur tokens Aiglon réels. |

**TOTAL : 84/100** — QUALIFIÉ

---

### 2.2 Inspired-Le Rosey — 81/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 10 | 20 | Reproduction PARFAITE des tokens Le Rosey. Bichromatique pur #182f66 + #ffffff. Radius 0 partout. Shadow 0 partout. Spacing 7-72px exactement calqué. Base font-size 17px conforme. EB Garamond + Playfair Display = les polices exactes du site de référence (ce sont des Google Fonts accessibles). La seule reproduction pixel-perfect de tokens dans tout le panel. |
| Alignement BISP | 8 | 16 | 8 blocs complets et bien intégrés. Le ton éditorial serif crée une gravitas "confiante" sans arrogance. L'épure bichromatique laisse le contenu respirer. Les 4 piliers sont clairement présentés. Le traitement "Le Rosey" donne à BISP une allure d'institution centenaire — c'est un positionnement ambitieux mais cohérent avec "14 ans d'excellence". |
| UX / Conversion | 8 | 16 | Navigation Le Rosey-style avec 5 items visibles, toggle FR/EN avec état actif (font-weight 700 + underline). CTA rectangulaire conforme radius 0. Parcours parent logique. Les boutons rectangulaires purs sont distinctifs. Carousel témoignages avec dots. Breakpoints 375-1440px (les plus complets). |
| Originalité | 7 | 14 | Le mockup est la reproduction la plus fidèle, ce qui limite légèrement l'originalité. L'adaptation est "Le Rosey mais pour BISP" plutôt qu'une réinterprétation créative. Les media queries `forced-colors` et `@media print` sont des bonus accessibilité rares. Moins d'images BISP que d'autres mockups. |
| Anti-slop + Accessibilité | 10 | 20 | EB Garamond + Playfair Display : polices distinctives et élégantes. Breakpoints les plus complets (375, 480, 768, 1024, 1440px). `@media (forced-colors: active)` = accessibilité supérieure. `@media print` = accessibilité supérieure. prefers-reduced-motion en CSS + JS. Focus visible 3px solid navy. Contraste excellent (navy sur blanc). Flat design pur = 0 distraction visuelle. |

**TOTAL : 81/100** — QUALIFIÉ (Meilleure accessibilité du panel)

---

### 2.3 Inspired-Sevenoaks — 79/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 8 | 16 | Teal #004f5d exact. Flat design conforme (0 shadows). Radius 0-3px + 9999px pill conforme. DM Sans comme proxy Bliss humaniste est un bon choix. Le hero split (vidéo gauche | teal droite) est une interprétation directe du hero split de Sevenoaks. Le H1 uppercase bold reproduit le style Bliss 50px/700 de Sevenoaks. |
| Alignement BISP | 8 | 16 | 8 blocs complets. Les 4 piliers bien présentés. Le teal est une couleur distinctive qui différencie BISP des écoles navy classiques. Le badge "32 nationalités depuis 2012" dans le hero est efficace. Le tone "international" et "concret" est bien capturé. La mosaïque photo dans les programmes est riche. |
| UX / Conversion | 8 | 16 | Navigation complète avec 5 items. Toggle FR/EN en pill border. CTA pill 9999px en teal. Le hero split met le contenu textuel dans un espace coloré dédié = lisibilité maximale. Parcours parent clair. prefers-reduced-motion utilise `no-preference` (best practice). Mobile menu overlay complet. |
| Originalité | 9 | 18 | Le hero split est le geste de design le plus audacieux et distinctif du panel. Aucun autre mockup n'a osé cette composition asymétrique. Le teal comme couleur primaire (plutôt que navy) est un choix créatif qui donne à BISP une identité fraîche et moderne. Les badges proof dans le hero (nationalités, campus) sont bien intégrés. |
| Anti-slop + Accessibilité | 7 | 14 | DM Sans : pas bannie mais très répandue (utilisation justifiée comme proxy Bliss). Pas de breakpoint 375px (major). Touch targets insuffisants sur éléments secondaires. prefers-reduced-motion en best practice (no-preference). 30 images avec alt texts. Flat design = contraste naturellement bon. |

**TOTAL : 79/100** — QUALIFIÉ

---

### 2.4 Inspired-Gordonstoun — 77/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 9 | 18 | Pourpre monochromatique #702381 exact. Lavande #c7b0d5 et gris #7a7d83 conformes. Le traitement CAPS/italic mixte (Josefin Sans caps + Cormorant Garamond italic dans le même titre) reproduit fidèlement la signature typographique Ivy Presto + Proxima Nova de Gordonstoun. Texture grain SVG = fidèle à l'esthétique texturée. Radius pill 50px conforme. |
| Alignement BISP | 7 | 14 | 8 blocs complets. Les 4 piliers présents. Le pourpre est un choix de couleur audacieux pour BISP — il ne s'ancre pas dans la palette existante (navy/orange). Le ton est plus "artistique/magazine" que "chaleureux/familial". Le traitement éditorial est sophistiqué mais pourrait aliéner les parents qui cherchent du concret plutôt que de l'esthétique. |
| UX / Conversion | 7 | 14 | Navigation complète, 5 items. Toggle FR/EN avec état actif en pourpre. CTA outline pill. Le hero place le contenu en bas (align-items: flex-end) = composition magazine. Parcours parent présent mais le pourpre dominant peut sembler froid. Menu mobile overlay en pourpre profond. |
| Originalité | 9 | 18 | Le traitement typographique mixed CAPS/italic est la signature la plus forte du panel après le hero split Sevenoaks. La texture grain body::before est un détail subtil qui ajoute de la tactilité. L'asymétrie de mise en page crée un rythme éditorial magazine. Le hero overlay pourpre (au lieu de navy) est distinctif. |
| Anti-slop + Accessibilité | 7 | 14 | Cormorant Garamond + Josefin Sans : polices distinctives, aucune bannie. Pas de breakpoint 375px (minor per critic — 480px used). 5 déclarations touch target 48px (bon). prefers-reduced-motion 3 blocs. Focus visible 3px lavande. La texture grain (z-index 9999) a `pointer-events: none` (vérifié). Skip-link fonctionnel. |

**TOTAL : 77/100** — QUALIFIÉ (4e position)

---

### 2.5 Inspired-Kent College — 76/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 9 | 18 | Rouge monochromatique #aa0040 exact. Corail #ff4951 exact. Les formes organiques (border-radius asymétrique `48% 52% 55% 45% / 50% 45% 55% 50%`) reproduisent fidèlement les photos découpées en cercles/formes de Kent College. Les dots décoratifs (.dot--coral, .dot--crimson) sont une signature Kent College pure. Montserrat comme proxy Azo Sans 100% sans-serif : conforme. |
| Alignement BISP | 7 | 14 | 8 blocs complets. Les 4 piliers bien présentés. Le rouge monochromatique est énergétique et distinctif mais crée une tension avec le positionnement "chaleureux/bienveillant" de BISP. Le rouge évoque plus la dynamique que la sérénité. La qualité du contenu est bonne (témoignages diversifiés, programmes détaillés). |
| UX / Conversion | 8 | 16 | Navigation complète. Toggle FR/EN avec pill active en crimson. CTA pill en corail = très visible. Touch targets 52px (supérieur au minimum). Les formes organiques humanisent l'interface. Parcours parent clair. Hamburger mobile 48x48px. Menu mobile overlay en crimson. |
| Originalité | 8 | 16 | Les formes organiques (cercles, blob shapes) sont uniques dans le panel. Les dots décoratifs créent un langage visuel distinctif. La combinaison crimson + corail évite le monochrome plat. Les images organiques (border-radius asymétrique) apportent chaleur et humanité que le rouge seul n'a pas. Section-label avec barre corail = efficace. |
| Anti-slop + Accessibilité | 7 | 14 | Montserrat : pas bannie mais très répandue. Touch targets 52px (le plus généreux). 7 focus-visible. prefers-reduced-motion complet avec video fallback. 28 images avec alt sémantiques. Pas de breakpoint 375px en @media (480px utilisé). Contraste crimson/blanc = bon. |

**TOTAL : 76/100** — QUALIFIÉ (5e position)

---

### 2.6 Inspired-Repton — 74/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 8 | 16 | Navy #3e4561 exact. Gold #988360 et bronze #93866c exacts. Shadows micro (0.1px, 0.5px) conformes tokens. Montserrat Light 300-400 comme proxy Gotham Light + Montserrat Light : bon choix. Le concept de timeline verticale (15px border) est une signature Repton bien comprise. Radius 2px, 6px, 50px pill conformes. |
| Alignement BISP | 7 | 14 | 8 blocs complets. Le "quiet luxury" typographique (font-weight 300 dominant) crée un ton raffiné et confiant. Le gold accent évoque le prestige sans arrogance. Les 4 piliers sont présents. Le ton est plus "prestige britannique" que "chaleureux cosmopolite" — un léger décalage avec le positionnement BISP. |
| UX / Conversion | 7 | 14 | Navigation complète. Toggle FR/EN textuel. **CTA nav min-height 44px au lieu de 48px** (issue WCAG majeure signalée par le Critic). Boutons pill gold = distinctifs. Le concept timeline est narratif. Parcours parent présent. prefers-reduced-motion masque la vidéo et affiche le poster (excellent). |
| Originalité | 8 | 16 | Le concept de timeline verticale dorée est narratif et guidé — il raconte un parcours plutôt qu'il n'affiche des blocs. Le "quiet luxury" typographique (poids ultra-légers) est un choix créatif distinctif. Le gold comme accent principal (au lieu de simple décoration) donne une identité chromatique propre. |
| Anti-slop + Accessibilité | 7 | 14 | Montserrat seule (1 famille) : risque de monotonie typographique mais bien utilisée en variant les poids. Issue WCAG : CTA nav 44px < 48px minimum. Pas de breakpoint 375px. prefers-reduced-motion excellent (video hidden, poster shown, reveal opacity 1). Focus visible 2px gold. Contraste navy+gold/blanc = bon. |

**TOTAL : 74/100** — QUALIFIÉ (6e position)

---

### 2.7 Inspired-École des Roches — 73/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 8 | 16 | Navy profond #0b1e3a exact. Gold #fdb82e exact. Shadow cinématique 136px blur conforme. Pills 9999px conformes. Radius 30px cards conformes. DM Sans comme proxy Gill Sans : acceptable. Source Sans 3 comme proxy Agrandir : acceptable. Les poids ultra-légers (font-weight 200-300) reproduisent l'élégance EDR. |
| Alignement BISP | 7 | 14 | 8 blocs complets. La profondeur cinématique crée une impression de prestige. Le gold sur navy est une combinaison classique "école d'excellence". Les 4 piliers sont présents. Le ton est "confiant" et "international" mais la profondeur sombre peut sembler distante plutôt que "chaleureuse". |
| UX / Conversion | 7 | 14 | Navigation complète. Toggle FR/EN en pill avec état actif. CTA gold = très visible. Breakpoint 1440px présent (un des rares). `@media print` = bonus accessibilité. Touch targets 52px sur boutons mais pas sur nav links. Menu mobile overlay navy. Les pills arrondis sont cohérents et agréables. |
| Originalité | 7 | 14 | La profondeur cinématique (shadow 136px) est un effet visuel unique dans le panel. Les pills 9999px partout créent une cohérence de forme. Le badge hero avec bordure gold semi-transparente est élégant. Mais le design est globalement un "navy + gold prestige" assez classique — moins de risque créatif que Aiglon, Sevenoaks ou Gordonstoun. |
| Anti-slop + Accessibilité | 8 | 16 | DM Sans + Source Sans 3 : aucune bannie. 35 images alt text (le plus du panel). `@media print` et prefers-reduced-motion 3 blocs = accessibilité supérieure. Breakpoint 1440px présent. Focus visible 3px gold. Animations hero avec keyframes fadeUp (CSS only) = performant. Nav links sans min-height explicite (minor). |

**TOTAL : 73/100** — QUALIFIÉ (7e position, juste au-dessus du seuil)

---

### 2.8 Inspired-Beau Soleil — 68/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 7 | 14 | Palette #002654 (navy), #0087c9 (sky-blue), #ffd931/#c4a35a (gold) conforme. Radius gamme large 2-50px conforme, pill 50px conforme. **MAIS** : ajout de shadows (subtle, card, elevated) alors que les tokens Beau Soleil sont flat design pur (aucune shadow). C'est une déviation significative de l'identité visuelle de la référence. Cormorant Garamond + DM Sans + Playfair Display = trio riche mais les polices Beau Soleil originales sont sangbleusans (custom sans-serif) + Roboto : l'impression visuelle diverge. |
| Alignement BISP | 8 | 16 | **Le contenu le plus riche du panel.** 8 blocs obligatoires + sections bonus (Galerie Band, Bilingual Split, Paris Location Band, Accreditations Band). Les textes sont les plus détaillés. Les 4 piliers ont des preuves chiffrées. Les 3 campus sont listés avec adresses. Le prix par niveau est affiché. Le ton est le plus "concret" du panel. |
| UX / Conversion | 7 | 14 | Navigation complète. **Utilise un micro-drapeau dans le toggle langue** (le brief interdit les drapeaux). CTA pill visible. Parcours parent excellent (le plus complet). Carousel témoignages avec dots. Le contenu bonus (galerie, bilingual split) enrichit le parcours mais allonge la page. **Pas de breakpoint 375px** (major). |
| Originalité | 6 | 12 | Le mockup est le plus conventionnel du panel. L'alternance blanc/navy est bien exécutée mais c'est le pattern le plus commun (7/9 sites de référence l'utilisent). Pas de geste de design audacieux comparable au hero split Sevenoaks, au dark cinématique Aiglon, ou au mixed typography Gordonstoun. Le layout est "propre mais prévisible". |
| Anti-slop + Accessibilité | 6 | 12 | Cormorant Garamond + DM Sans + Playfair Display : polices non bannies mais DM Sans est très répandue. Pas de breakpoint 375px ni 1440px. Touch targets partiels (nav links sans min-height). Drapeau dans le toggle = déviation du brief. Le contenu est excellent mais le design est le moins distinctif. Les shadows ajoutées contredisent les tokens flat design de Beau Soleil. |

**TOTAL : 68/100** — NON QUALIFIÉ (sous le seuil de 70/100)

---

### 2.9 Inspired-Haut-Lac — 67/100

| Critère | Score /10 | Pondéré | Justification |
|---------|:---------:|:-------:|---------------|
| Fidélité référence | 7 | 14 | Palette multi-accent teal #348397, red #ed3122, vert #429e7b, orange #d89137 conforme. Montserrat (headings) + Be Vietnam Pro (body) = polices exactes Haut-Lac. Radius 3, 5, 12px conforme (max 12px). Border thick 5px conforme. Le concept de diagonales est mentionné mais la mise en œuvre dans le CSS est moins spectaculaire que sur le site Haut-Lac réel (qui utilise des coupes diagonales très marquées avec clip-path). |
| Alignement BISP | 7 | 14 | 8 blocs complets. Les 4 piliers présents. La palette multi-accent est énergétique et "internationale". Le teal + red est distinctif. Mais la multiplicité des couleurs (4 accents) peut diluer l'identité BISP plutôt que la renforcer. Le design brief recommande une "palette resserrée (2-5 couleurs max)" — 4 accents + neutrals pousse la limite. |
| UX / Conversion | 7 | 14 | Navigation complète. Toggle FR/EN textuel. CTA en red = très visible. Touch targets 48px (4 déclarations). Mobile menu avec close button 48x48. Le hero utilise une bande diagonale teal. Parcours parent clair. Pas de breakpoint 375px en @media. Le fichier est le plus long (3028 lignes) = complexité potentielle. |
| Originalité | 6 | 12 | Les diagonales sont mentionnées dans le CSS mais moins marquées visuellement que sur le Haut-Lac réel. La palette multi-accent est colorée mais pas aussi maîtrisée que l'original. Les pastilles numérotées de Haut-Lac ("What matters to us") ne sont pas reproduites. Le traitement B&W des photos (signature Haut-Lac) est CSS-ready mais dépend des images. L'adaptation est correcte mais manque de l'énergie visuelle du site original. |
| Anti-slop + Accessibilité | 7 | 14 | Montserrat + Be Vietnam Pro : polices exactes Haut-Lac, non bannies. prefers-reduced-motion 4 blocs (le plus détaillé du panel). Focus visible 3px teal-light. Touch targets 48px. Pas de breakpoint 375px. Le fichier le plus long = potentiel de maintenance. Tokens bien ancrés mais l'exécution manque de polish par rapport aux 3 premiers. |

**TOTAL : 67/100** — NON QUALIFIÉ (sous le seuil de 70/100)

---

## 3. Top 3 forces / Top 3 faiblesses par mockup

### Aiglon (84/100)
**Forces** : (1) Ambiance cinématique sombre immersive = émotion immédiate ; (2) Traitement "red accent words" dans les titres = signature unique ; (3) Trio typographique Satoshi + Cabinet Grotesk + Instrument Serif = richesse sans chaos
**Faiblesses** : (1) L'ambiance sombre peut sembler intimidante pour le pilier "chaleureux" ; (2) Pas de breakpoint 1440px ; (3) Skip-link nommé `.skip-to-content` au lieu du conventionnel `.skip-link`

### Le Rosey (81/100)
**Forces** : (1) Reproduction parfaite des tokens (radius 0, shadow 0, bichromatique pur) ; (2) Breakpoints les plus complets (375-1440px) + forced-colors + print ; (3) Élégance éditoriale serif = gravitas institutionnelle
**Faiblesses** : (1) Originalité limitée (trop fidèle = peu de réinterprétation créative) ; (2) Moins d'images BISP que d'autres mockups ; (3) Carousel dépend de JS sans fallback no-JS

### Sevenoaks (79/100)
**Forces** : (1) Hero split = geste de design le plus audacieux du panel ; (2) Teal comme primaire = identité fraîche vs. navy classique ; (3) prefers-reduced-motion en best practice (no-preference)
**Faiblesses** : (1) Pas de breakpoint 375px (major) ; (2) Touch targets insuffisants sur éléments secondaires ; (3) DM Sans seule police = légèrement générique

### Gordonstoun (77/100)
**Forces** : (1) Mixed CAPS/italic typography = signature typographique la plus forte ; (2) Texture grain SVG = tactilité unique ; (3) Layout asymétrique magazine = rythme éditorial
**Faiblesses** : (1) Pourpre pas ancré dans la palette BISP existante ; (2) Ton plus "artistique" que "familial/chaleureux" ; (3) Pas de breakpoint 375px

### Kent College (76/100)
**Forces** : (1) Formes organiques (blob border-radius) = humanisant et unique ; (2) Dots décoratifs = langage visuel distinctif ; (3) Touch targets 52px (le plus généreux)
**Faiblesses** : (1) Rouge monochromatique = tension avec "chaleureux/bienveillant" ; (2) Montserrat seule = répandue ; (3) Pas de breakpoint 375px en @media

### Repton (74/100)
**Forces** : (1) Quiet luxury typographique (font-weight 300) = prestige discret ; (2) Concept timeline narratif = guidé ; (3) Gold comme accent principal = identité chromatique forte
**Faiblesses** : (1) CTA nav 44px < 48px WCAG minimum ; (2) Monotonie typographique (Montserrat seule) ; (3) Pas de breakpoint 375px

### École des Roches (73/100)
**Forces** : (1) Shadow cinématique 136px = profondeur unique ; (2) 35 images alt text (le plus du panel) ; (3) Breakpoint 1440px + @media print
**Faiblesses** : (1) Design "navy + gold prestige" classique, peu de risque créatif ; (2) Nav links sans min-height explicite ; (3) Poids ultra-légers (200-300) = risque de lisibilité

### Beau Soleil (68/100)
**Forces** : (1) Contenu le plus riche et le plus complet du panel ; (2) Sections bonus (galerie, bilingual split, Paris band) ; (3) Ton le plus "concret" avec prix et adresses
**Faiblesses** : (1) Shadows ajoutées contredisant les tokens flat design Beau Soleil ; (2) Drapeau dans le toggle langue (interdit par le brief) ; (3) Layout le plus conventionnel, manque de geste créatif

### Haut-Lac (67/100)
**Forces** : (1) prefers-reduced-motion 4 blocs (le plus détaillé) ; (2) Palette multi-accent énergétique ; (3) Tokens polices exactes (Montserrat + Be Vietnam Pro)
**Faiblesses** : (1) Diagonales moins marquées que le Haut-Lac réel ; (2) 4 accents diluent l'identité plus qu'ils ne la renforcent ; (3) Fichier le plus long (3028 lignes) = complexité

---

## 4. Head-to-Head — Meilleur mockup par aspect

| Aspect | Meilleur mockup | Pourquoi |
|--------|-----------------|----------|
| **Hero** | **Sevenoaks** | Le hero split (vidéo | teal) est le geste le plus audacieux. Composition asymétrique mémorable, contenu textuel sur fond coloré = lisibilité maximale. Aiglon en 2e (cinématique sombre + red words). |
| **Navigation** | **Le Rosey** | La plus élégante. Serif EB Garamond, rectangulaire pur (radius 0), transition transparent → solid subtile. Hauteur nav 85px → 72px au scroll. La plus "institution d'excellence". |
| **Typographie** | **Gordonstoun** | Le traitement mixed CAPS/italic (Josefin Sans caps + Cormorant Garamond italic dans le même titre) est la signature typographique la plus distinctive. Aiglon en 2e (trio Satoshi/Cabinet/Instrument). |
| **Couleurs** | **Aiglon** | La palette dark cinématique (#0d1117, #b11d23, #ceab52) est la plus émotionnellement impactante. Le contraste entre le fond sombre, le rouge vif et l'or crée une tension visuelle qui capture immédiatement l'attention. Le Rosey en 2e (pureté bichromatique). |
| **Layout** | **Aiglon** | L'alternance entre sections sombres et les wave separators crée un rythme narratif. Les cards de programmes avec image + body + meta sont bien structurées. Gordonstoun en 2e (asymétrie magazine). |
| **Contenu** | **Beau Soleil** | Le contenu le plus riche : sections bonus (galerie, bilingual split, Paris location band), prix par niveau, adresses des 3 campus, 3 témoignages détaillés. Le meilleur parcours informatif pour un parent. Aiglon en 2e (6 témoignages, programme détaillé). |
| **Émotion** | **Aiglon** | L'ambiance cinématique sombre crée l'émotion la plus immédiate et la plus mémorable. Les mots rouges dans les titres ("langues", "élèves", "monde") ajoutent une couche de storytelling. Sevenoaks en 2e (le split hero est frappant). |
| **UX** | **Aiglon** | Le seul avec breakpoint 375px + floating CTA mobile + escape key ferme le menu + carrousel prev/next + 6 témoignages. Le plus complet en terme de parcours interactif. Le Rosey en 2e (breakpoints les plus complets techniquement). |

---

## 5. Classement final des 9

| Rang | Mockup | Score | Statut | Commentaire |
|:----:|--------|:-----:|:------:|-------------|
| **1** | **Inspired-Aiglon** | **84** | QUALIFIÉ | Le meilleur équilibre fidélité-originalité-UX-émotion. Phase 2. |
| **2** | **Inspired-Le Rosey** | **81** | QUALIFIÉ | Le plus pur techniquement, le plus accessible. Phase 2. |
| **3** | **Inspired-Sevenoaks** | **79** | QUALIFIÉ | Le plus audacieux visuellement (hero split). Phase 2. |
| 4 | Inspired-Gordonstoun | 77 | Éliminé | Signature typo forte mais pourpre hors palette BISP. |
| 5 | Inspired-Kent College | 76 | Éliminé | Formes organiques uniques mais rouge trop agressif. |
| 6 | Inspired-Repton | 74 | Éliminé | Quiet luxury élégant mais issue WCAG 44px. |
| 7 | Inspired-École des Roches | 73 | Éliminé | Bon mais trop classique, peu de risque créatif. |
| 8 | Inspired-Beau Soleil | 68 | Éliminé | Meilleur contenu mais design trop conventionnel. |
| 9 | Inspired-Haut-Lac | 67 | Éliminé | Tokens fidèles mais exécution sous le niveau. |

---

## 6. RECOMMANDATION HYBRIDE pour Phase 2

### La vision : "Aiglon Cinematic + Rosey Editorial + Sevenoaks Bold"

Prendre les meilleurs éléments de chaque mockup qualifié et les fusionner en un design hybride BISP unique :

| Composant | Prendre de... | Pourquoi |
|-----------|---------------|----------|
| **Hero** | **Sevenoaks** (split vidéo \| couleur) | Le geste de design le plus mémorable. Adapter : vidéo gauche 55% \| navy BISP droite 45% avec le contenu textuel. Le split crée une entrée immédiate dans l'univers BISP sans dépendre de la qualité vidéo seule. |
| **Navigation** | **Le Rosey** (serif élégante, rectangulaire) | La plus institutionnelle et lisible. EB Garamond pour les liens nav donne une gravitas unique. Adapter : radius 0 sur la nav mais pills sur les CTA pour contraste. |
| **Typographie titres** | **Aiglon** (Cabinet Grotesk display + red accent words) | Le traitement "mots-clés en couleur accent" dans les titres est la technique de storytelling la plus efficace. Adapter : utiliser la couleur accent BISP (gold ou teal) au lieu du rouge Aiglon. |
| **Typographie corps** | **Le Rosey** (EB Garamond serif) | Le serif comme police de corps donne une lisibilité éditoriale et une distinction immédiate vs. le sans-serif générique de 90% des sites d'école. Base 17px, line-height 1.57. |
| **Typographie accent** | **Aiglon** (Instrument Serif italic) | Pour les citations, témoignages et le mot du directeur. Le serif italic crée un contraste émotionnel avec le display bold des titres. |
| **Palette primaire** | **Aiglon** structure + **Le Rosey** épure | Navy profond BISP (#1a2744) comme dominante. Blanc pur (#ffffff) et crème (#f5f0eb) comme fonds alternés. Palette resserrée à 2 couleurs max + 1 accent. |
| **Couleur accent** | **Sevenoaks** teal (#004f5d) OU gold (#c4a35a) | Le teal de Sevenoaks différencie BISP de toutes les écoles navy+rouge/or classiques. Alternative : gold pour plus de prestige. Décision à valider avec le directeur en Phase 6a. |
| **Sections sombres** | **Aiglon** (dark cinematic) | Les sections Chiffres Clés et Programmes sur fond sombre (#0d1117 ou navy profond) avec texte blanc. Les stats animées sur fond sombre sont spectaculaires. |
| **Sections claires** | **Le Rosey** (bichromatique blanc/crème) | Les sections Promesses, Témoignages et Directeur sur fond blanc ou crème. L'espace blanc généreux (spacing 72px Le Rosey) laisse le contenu respirer. |
| **Contenu** | **Beau Soleil** (richesse) | Reprendre les sections bonus : bilingual split, Paris location band avec 3 campus, accreditations band. Le contenu de Beau Soleil est le plus complet pour un parent. |
| **Promesses** | **Aiglon** (cards sur fond dark) | Les promise-cards d'Aiglon avec icônes SVG + preuve chiffrée en accent rouge/gold sont les plus impactantes. |
| **Programmes** | **Aiglon** (cards avec image + body + meta + prix) | Structure programme la plus complète : image, badge âge, cycle, titre avec accent word, description, prix, lien découvrir. |
| **Témoignages** | **Aiglon** (6 témoignages, carousel prev/next) | Le plus diversifié (6 nationalités) et le mieux structuré (avatar initiales + nom + détail). Adapter le carousel en scroll horizontal natif. |
| **Directeur** | **Aiglon** (2 colonnes, portrait + blockquote avec signature) | Structure claire et respectueuse. L'Instrument Serif italic pour la citation crée une distinction éditoriale. |
| **CTA final** | **Sevenoaks** (aplat couleur pleine largeur, H2 uppercase bold) | "PRÊT À DÉCOUVRIR BISP ?" en uppercase bold sur fond teal/navy = mémorable. Deux CTAs : "Planifier ma visite" + numéro de téléphone. |
| **Footer** | **Le Rosey** (navy, serif, 4 colonnes, accréditations) | Structure Rosey adaptée : 5 colonnes (brand, école, programmes, admissions, campus). Logos Cambridge + Pearson. Toggle FR/EN. |
| **Formes** | **Le Rosey** (radius 0 dominant) + **Sevenoaks** (pills CTA) | Angles vifs sur les conteneurs et cartes (radius 0-3px), pills exclusivement sur les boutons CTA. Ce contraste forme/action est le plus efficace du panel. |
| **Shadows** | **Aiglon** (dramatiques sur cards, aucune ailleurs) | Les shadows 29px ne s'appliquent qu'aux éléments en hover/focus. Le design de base reste plat. |
| **Animations** | **Aiglon** (reveal + counters + stagger) | IntersectionObserver pour les reveals, counters animés pour les stats, stagger pour les grilles. CSS-only pour la page de base, JS progressive enhancement. |
| **Breakpoints** | **Le Rosey** (375, 480, 768, 1024, 1440px) | Les plus complets. + forced-colors + @media print de Le Rosey. |
| **Mobile CTA** | **Aiglon** (floating CTA sticky) | Le floating CTA mobile qui apparaît après le hero = conversion maximale sur mobile. |

### Résumé de la formule hybride

> **"Un site noir et blanc éditorial (Le Rosey) qui s'ouvre avec un hero split audacieux (Sevenoaks), utilise des accents colorés dans les titres (Aiglon), plonge dans des sections cinématiques sombres (Aiglon) pour les chiffres et les programmes, et fournit le contenu le plus riche (Beau Soleil) — le tout dans la police la plus élégante du panel (EB Garamond + Cabinet Grotesk)."**

---

## 7. Fixes critiques pour Phase 2

### Priorité 1 — WCAG (bloquants)

| # | Fix | Source | Effort |
|---|-----|--------|--------|
| 1 | Ajouter breakpoints 375px et 1440px à tous les mockups | Critic audit | Moyen |
| 2 | Tous les éléments interactifs doivent avoir min-height: 48px (CTA nav Repton à 44px) | WCAG 2.5.5 | Faible |
| 3 | Touch targets 48x48px sur TOUS les éléments cliquables (nav links, lang toggle, social links) | WCAG 2.5.5 | Moyen |

### Priorité 2 — Brief compliance

| # | Fix | Source | Effort |
|---|-----|--------|--------|
| 4 | Retirer tout micro-drapeau du toggle FR/EN (Beau Soleil) | Design brief | Faible |
| 5 | Harmoniser le naming des classes skip-link (.skip-link partout, pas .skip-to-content) | Convention | Faible |
| 6 | Ajouter fallback no-JS pour les carousels (Le Rosey, Aiglon) | Best practice | Moyen |

### Priorité 3 — Enrichissement

| # | Fix | Source | Effort |
|---|-----|--------|--------|
| 7 | Intégrer les sections bonus de Beau Soleil (bilingual split, Paris band, galerie) dans le mockup hybride | Scoring | Élevé |
| 8 | Porter le nombre de témoignages à 6 minimum avec diversité de nationalités (modèle Aiglon) | Scoring | Moyen |
| 9 | Ajouter `@media (forced-colors: active)` et `@media print` (modèle Le Rosey) | Accessibilité | Faible |
| 10 | Tester le contraste de TOUTES les combinaisons couleur/fond avec un outil automatisé | WCAG | Moyen |

---

## 8. Checklist livrables Phase 2

- [ ] **Mockup hybride v1** : HTML single-file intégrant les composants recommandés ci-dessus
- [ ] **Validation breakpoints** : testé à 375px, 480px, 768px, 1024px, 1440px
- [ ] **Audit WCAG automatisé** : Lighthouse score > 90 sur accessibilité
- [ ] **Contraste vérifié** : toutes combinaisons couleur/fond à 4.5:1 minimum
- [ ] **Touch targets vérifié** : 48x48px sur tous les éléments interactifs
- [ ] **Contenu complet** : 8 blocs obligatoires + sections bonus (bilingual, Paris, galerie)
- [ ] **6 témoignages** : 6 nationalités diversifiées minimum
- [ ] **Toggle FR/EN** : textuel, sans drapeau, avec état actif clair
- [ ] **prefers-reduced-motion** : complet avec fallback statique
- [ ] **@media forced-colors** : présent
- [ ] **@media print** : présent
- [ ] **Skip-link** : `.skip-link` nommé uniformément
- [ ] **Palette finale validée** : navy BISP + accent (teal OU gold) — décision post-session directeur
- [ ] **Polices finales** : EB Garamond (display/body serif) + Cabinet Grotesk (headings display) + Instrument Serif (accent éditorial)
- [ ] **Screenshots 1440px** : capturés pour comparaison avec les références
- [ ] **Revue directeur** : présentation du mockup hybride pour validation ton/palette avant déploiement

---

*Fin du scoring report. Les 3 mockups qualifiés (Aiglon, Le Rosey, Sevenoaks) passent en Phase 2 pour hybridation. Les 6 autres sont éliminés mais leurs meilleurs éléments sont intégrés dans la recommandation hybride.*
