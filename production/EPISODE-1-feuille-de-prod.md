# ÉPISODE 1 — FEUILLE DE PRODUCTION
## Tous les prompts, dans l'ordre d'exécution

Copie opérationnelle : tout ce qui se colle dans Higgsfield est ici, dans l'ordre. Le raisonnement derrière chaque choix reste dans `cirque-90s.md`, `seedance-animation.md` et `tto-mascotte.md` — si vous modifiez un prompt, modifiez-le **aux deux endroits**.

Partout : `nano_banana_pro` pour les images, `9:16` sauf mention contraire, `2k`, 2 crédits par image.

---

## ⚠️ DEUX CORRECTIONS AVANT DE COMMENCER

### 1. Les phrases du hook ne tiennent pas dans leurs cases

La charte alloue 3 secondes à la phrase choc et 3 à la phrase réponse. Vérification faite :

| | Mots | Besoin réel | Alloué | Débit imposé |
|---|---|---|---|---|
| ① Phrase choc | 11 | 5,5 s | 3 s | **220 mots/min** |
| ⑤ Phrase réponse | 18 | 7,2 s | 3 s | **360 mots/min** |

Une narration lisible tient entre 140 et 160 mots/minute, et une voix grave et posée descend plutôt vers 120. À 360, la phrase réponse est physiquement indisponible — aucune voix ne la dira.

**Solution retenue : élargir les cases plutôt qu'amputer les phrases.** Le hook passe de 13 à 16 secondes.

```
① phrase choc      0:00 → 0:05      (5 s, ~130 mots/min)
② pause            0:05 → 0:06      (0,8 s de silence)
③ défilé           0:06 → 0:10      (11 plans à 0,36 s)
④ impact           0:10 → 0:11
⑤ phrase réponse   0:11 → 0:15      (4 s — voir phrase raccourcie ci-dessous)
⑥ cloche + lockup  0:15 → 0:16
```

La phrase réponse est raccourcie pour tenir en 4 secondes sans perdre son sens :

> ~~« Et ce chiffre vient d'un sergent de cavalerie qui cherchait juste à ne pas tomber de son cheval. »~~
> **« Et ce chiffre vient d'un sergent de cavalerie. »** — 8 mots, 3,2 s à 150 mots/min ✓

La subordonnée perdue n'est pas gâchée : elle est déjà dite au début de l'acte 1, où elle a la place de respirer.

**Durée du film : 16 s de hook + 1:44 = 2:00.**

### 2. Les trois effets sonores ne sont pas générables sur Higgsfield

La charte les annonce « générables en text-to-audio ». C'est inexact : Higgsfield réserve `sonilo_music` et `mirelo_text_to_audio` au pipeline de génération de jeux, et interdit leur usage en audio autonome. `seed_audio` ne fait que de la parole.

**Il faut donc les prendre ailleurs** — une banque de sons libres de droits (Freesound, Pixabay Sound, Epidemic Sound selon votre licence). Trois fichiers à trouver une fois, réutilisés à vie :

| Son | Durée | Ce qu'il faut chercher |
|---|---|---|
| Pulse du défilé | ~4 s | battement rythmique sourd, montée en intensité, sans mélodie |
| Impact de fin | ~1 s | whoosh descendant ou coup sourd avec queue de réverbe |
| Cloche | ~1,5 s | cloche claire, résonance longue, une seule frappe |

---

## ÉTAPE 1 — VALIDATION DU STYLE · 6 crédits

Générez ces trois-là **et arrêtez-vous**. Ce sont les trois cas où la gravure peut casser : une silhouette humaine en pied, une foule dense en contre-plongée, un corps en vol. S'ils tiennent, tout le reste tiendra.

Le bloc de style est identique partout — c'est lui qui tient la cohérence, ne le modifiez jamais.

**□ Plan 3 — silhouette d'officier**
> A 19th-century lithographic engraving, tall vertical composition: the full-length silhouette of an 18th-century cavalry officer in tall boots and long coat, standing backlit in a tall narrow stable doorway that fills the height of the frame, face not visible, straw and dust suspended in the light. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 9 — le Cirque Napoléon**
> A 19th-century lithographic engraving, tall vertical composition: seen from the ring floor looking steeply up, the tiered balconies of an ornate 1850s Paris circus rising in stacked rings above the viewer, packed with a crowd in silhouette, chandeliers and heavy velvet drapery overhead. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 11 — le corps en vol** ⭐
> A 19th-century lithographic engraving, tall vertical composition: the moment of release — a human body in mid-air, pure silhouette, arms extended, suspended in a tall empty shaft of light, one trapeze bar leaving the top of the frame and another entering from the side, nothing at all beneath, deep void filling the lower half. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**→ Point de décision.** Regardez-les en plein écran sur téléphone. Si le trait gravé et le grain de papier sont là, continuez. Sinon, dites-moi ce que vous voyez et je corrige le bloc de style avant que vous n'engagiez 20 crédits de plus.

---

## ÉTAPE 2 — LES 10 IMAGES RESTANTES · 20 crédits

**□ Plan 1 & 14 — la piste vide** *(le même fichier sert aux deux)*
> A 19th-century lithographic engraving, vertical composition: a top-down view of an empty circular circus ring, the perfect circle centred and filling the frame width, raked sawdust inside, deep darkness above and below the ring. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 2 — macro sciure**
> A 19th-century lithographic engraving, vertical composition: an extreme close-up of sawdust grains and a worn wooden circus ring border running across the lower third, shallow depth of field, darkness above. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 4 — le cavalier debout**
> A 19th-century lithographic engraving, tall vertical composition: seen from a low angle looking up, a standing rider in silhouette balanced upright on the back of a galloping horse, the rider's full height occupying the upper frame, sky and dust behind. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 5 — les sabots**
> A 19th-century lithographic engraving, vertical composition: a very low ground-level angle of galloping hooves throwing up earth in a curved arc towards the top of the frame, sense of speed and motion. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 6 — le fouet**
> A 19th-century lithographic engraving, vertical composition: a long training whip uncoiling away from the viewer into deep perspective, receding from the foreground towards a distant circular ring edge, sawdust disturbed along its path, strong depth from bottom to top of frame. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 7 — les galeries**
> A 19th-century lithographic engraving, tall vertical composition: looking up at the stacked wooden galleries of an 18th-century amphitheatre, three tiers rising one above the other, packed with a crowd in silhouette, gaslight glow. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 8 — musiciens et clown**
> A 19th-century lithographic engraving, vertical composition: musicians and a clown in period costume seen from behind, walking away from the viewer into a lit circular ring, staggered in depth from foreground to background, dust suspended in the light beams. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 10 — les mains sur la barre**
> A 19th-century lithographic engraving, vertical composition: an extreme close-up of chalked hands gripping a wooden trapeze bar, forearms rising vertically out of the top of the frame, tension visible in the fingers and tendons, darkness below. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 12 — le maillot**
> A 19th-century lithographic engraving, vertical composition: a one-piece knitted garment laid flat on a wooden table seen from directly above, the garment running vertically down the length of the frame, lit from the side, folds and knit texture visible. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Plan 13 — l'acrobate sur tissus**
> A 19th-century lithographic engraving, tall vertical composition: a contemporary aerial acrobat suspended on hanging silks, the silks descending from the very top of the frame and trailing out of the bottom, a single vertical beam of light, pure silhouette, surrounding darkness, no props. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

---

## ÉTAPE 3 — IDENTITÉ DE CHAÎNE · 6 crédits, une seule fois

Ces trois images servent à **tous** les épisodes. Générées une fois, conservées, jamais régénérées. Format **1:1**, pas 9:16 — un carré se recadre dans les deux sens sans perte.

**□ Mascotte — l'Arpenteur** *(aspect `1:1`)*
> A 19th-century lithographic engraving, square emblem composition: the full-length silhouette of a lone figure in a long coat and wide-brimmed hat, seen in complete backlit silhouette with absolutely no facial features visible, standing in profile and holding up a pair of brass dividers in one hand as if measuring something distant. Centred, symmetrical, generous clean margins, strong readable silhouette against a plain luminous background. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No face, no eyes, no facial detail, no text, no captions, no watermark.

**□ Mascotte — variante main et compas** *(aspect `1:1`)*
> A 19th-century lithographic engraving, square emblem composition: a single hand holding a pair of brass dividers open above a plain surface, seen from a slightly raised angle, the points of the dividers resting precisely on the surface. No arm beyond the wrist, no figure, no person. Centred, symmetrical, generous clean margins. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**□ Logo TTO** *(aspect `1:1`)*
> A logo mark: the three letters "TTO" as a centred monogram, engraved 19th-century letterpress style, bold condensed serif capitals with fine cross-hatching inside the letterforms, enclosed in a thin engraved circular rule. Ink black on aged cream paper with subtle fibre and foxing, one small crimson accent. Flat, centred, symmetrical, high contrast, clean margins. Only the letters T, T and O — no other text, no tagline, no watermark.

**Contrôles :** sur les mascottes, aucun visage ne doit apparaître et le compas doit se lire comme un compas. Sur le logo, vérifiez **exactement T-T-O** — ni « TT0 », ni « TIO ». C'est le seul défaut qui disqualifie un logo.

**Départage des deux mascottes :** réduisez-les à 100 pixels côte à côte. Celle que vous reconnaissez encore gagne.

---

## ÉTAPE 4 — VOIX OFF · `seed_audio`

Choisissez **une** voix dans `list_voices` et gardez la même pour les six prises. Une voix qui change entre deux actes s'entend immédiatement.

Six prises séparées plutôt qu'une longue : si une seule est ratée, vous ne refaites qu'elle.

**□ Prise H1 — phrase choc** *(à descendre de 2 à 4 demi-tons au montage, pas à la génération)*
> Toutes les pistes de cirque du monde font exactement treize mètres.

**□ Prise H2 — phrase réponse** *(voix normale, aucun effet)*
> Et ce chiffre vient d'un sergent de cavalerie.

**□ Prise A1 — acte 1**
> Philip Astley découvre qu'en galopant en cercle, debout sur le dos de son cheval, la force centrifuge l'aide à tenir en équilibre. En ligne droite, c'est impossible. Il lui faut donc une piste ronde. Il la fixe à treize mètres — la portée exacte de son fouet depuis le centre. Puis il comprend qu'un spectacle de chevaux ne remplit pas une soirée. Alors il engage des musiciens, des clowns, des acrobates. Des gens pour occuper le public pendant que les chevaux se reposent. Le cirque moderne vient de naître. Et l'acrobate y est un bouche-trou.

**□ Prise A2 — acte 2**
> 12 novembre 1859, Cirque Napoléon, Paris. Un Toulousain de vingt-et-un ans s'élance d'une plateforme, lâche sa barre, et attrape la suivante en plein vol. Personne n'a jamais fait ça. Napoléon III vient le voir. Pour son numéro, il a dessiné un vêtement moulant d'une seule pièce. Il l'appelle simplement « le maillot ». Il meurt onze ans plus tard. Et c'est après sa mort que les Anglais donnent son nom à ce vêtement. Il s'appelait Jules Léotard.

**□ Prise A3 — acte 3**
> Un siècle plus tard, les animaux sont contestés, puis interdits. En 1984, une troupe québécoise monte un spectacle sans une seule bête. Rien que des corps humains. Le bouche-trou de 1768 est devenu le spectacle tout entier.

**□ Prise A4 — chute**
> Tout a changé. Sauf les treize mètres. Et toi, tu l'avais remarqué ?

⚠️ **Les deux premières lignes de l'ancien script sont supprimées** — elles sont désormais portées par les prises H1 et H2 du hook. Ne les enregistrez pas deux fois.

**Contrôle de durée :** la prise A1 doit tenir ~41 s, A2 ~30 s, A3 ~16 s, A4 ~5 s. Si une prise dépasse nettement, ajustez `speech_rate` plutôt que de couper du texte.

---

## ÉTAPE 5 — ANIMATION SEEDANCE *(optionnelle)*

Les 14 prompts de mouvement sont dans `seedance-animation.md`. Avant de vous y engager, relisez-en le budget : **~292 crédits**, soit onze fois le coût des images fixes.

**Testez d'abord sur le seul plan 11.** ~22,5 crédits. Si la gravure tremble sous le mouvement, vous l'aurez appris pour 22 crédits au lieu de 292.

Si vous renoncez à Seedance, le film fonctionne parfaitement en images fixes avec un zoom lent au montage — c'était le plan initial, et il coûte 26 crédits au lieu de 318.

---

## ÉTAPE 6 — MONTAGE

- **Voix off d'abord**, images calées dessus ensuite.
- **Coupes franches**, aucune transition.
- **Sous-titres incrustés** sur 100 % de la durée. ⚠️ Le fichier `13-metres.srt` est calé sur la version **sans hook TTO**. Avec le hook, décalez tout de +16 s et ajoutez les deux phrases du hook en tête — dites-le-moi, je regénère le fichier calé.
- **Plans 1 et 14 rigoureusement identiques.** C'est le bouclage qui déclenche le replay.
- **Cloche exactement sur l'apparition du lockup**, ni avant ni après.

---

## RÉCAPITULATIF DES COÛTS

| Étape | Crédits |
|---|---|
| 1 — Validation du style (3 images) | 6 |
| 2 — Images restantes (10) | 20 |
| 3 — Identité de chaîne (3, une seule fois) | 6 |
| 4 — Voix off (6 prises) | à mesurer |
| 5 — Animation Seedance *(optionnelle)* | ~292 |
| **Total sans animation** | **32 + voix** |
| **Total avec animation** | **~324 + voix** |

Solde disponible : 356 crédits.

Sans l'animation, l'épisode coûte moins de 10 % de votre solde et vous laisse de quoi produire une dizaine d'épisodes. Avec, il en consomme 91 % — et l'identité de chaîne, elle, est payée une seule fois pour toujours.
