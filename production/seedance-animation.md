# « 13 MÈTRES » — dossier d'animation Seedance 4K
## Image-to-video · 9:16 · 14 plans

Ce dossier complète `cirque-90s.md`. Celui-là décrit les **images fixes** ; celui-ci décrit comment les **animer**.

Le principe : Seedance ne génère pas les plans à partir de rien. Chaque image fixe validée sert de **première frame**, et Seedance l'anime. C'est le mode image-to-video, et c'est le seul acceptable ici — voir la section « Le vrai risque » plus bas.

---

## ⚠️ BUDGET — à lire avant de lancer quoi que ce soit

| Poste | Détail | Crédits |
|---|---|---|
| 13 images fixes | `nano_banana_pro` 9:16 2k, 2 crédits pièce | **26** |
| 13 animations | `seedance_2_0`, ~22,5 crédits pièce | **~292** |
| Upscale 4K | si non natif, ~coût à confirmer | **?** |
| **Total** | | **~318 minimum** |

**Solde disponible : 356 crédits.** L'opération en consomme environ **89 %**, sans compter la voix off ni le moindre plan raté.

Le coût par plan animé est **onze fois** celui d'une image fixe. Un plan refait pour cause de tremblement coûte 22,5 crédits, pas 2. À ce tarif, trois ratés effacent la marge.

**Les chiffres marqués `~` sont issus de ma connaissance du catalogue, pas d'une lecture en direct** — l'accès Higgsfield m'est fermé. Vérifiez le coût réel de `seedance_2_0` en 4K avant de vous engager : un écart de 5 crédits par plan déplace le total de 65 crédits.

### Le chemin que je recommande, par paliers

1. **Palier 1 — 2 crédits.** Générez l'image fixe du plan 11.
2. **Palier 2 — ~22,5 crédits.** Animez ce seul plan. Regardez-le en plein écran, sur téléphone.
3. **Décision.** Si la gravure tient sans trembler, continuez. Sinon vous avez perdu 24 crédits au lieu de 318.
4. **Palier 3.** Les 12 images restantes (24 crédits), puis les animations par groupes de quatre, en contrôlant à chaque groupe.

Le plan 11 est le bon juge : un corps humain en vol, sur fond de vide, en hachures fines. Si Seedance le tient, il tiendra le reste.

---

## LE VRAI RISQUE : la gravure sous le mouvement

Il faut le dire franchement, parce que ça décide de la façon d'écrire les prompts.

Une lithographie XIXe est faite de **hachures croisées très fines**. Un modèle vidéo interpole entre les frames : ces hachures se mettent à « nager », le grain de papier scintille, les contours se déforment. C'est le défaut classique de l'animation générée sur du trait gravé, et il est d'autant plus visible que la texture est fine — donc maximal ici.

Trois règles en découlent, appliquées dans les 14 prompts ci-dessous.

**1. Le mouvement vient de la caméra, pas du sujet.** Un lent travelling avant sur une gravure fixe est stable. Un cheval dont on anime les jambes se déforme. Partout où c'est possible, le prompt décrit un mouvement d'appareil et un sujet immobile.

**2. Seuls les éléments diffus bougent.** Poussière en suspension, fumée, tissu qui frémit, lumière qui vacille. Ces éléments n'ont pas de contour net, donc leur déformation ne se voit pas. C'est là qu'on met la vie.

**3. Le négatif est aussi important que le positif.** Chaque prompt bannit explicitement le morphing, le scintillement et la dérive de style.

### Les trois plans à haut risque

| Plan | Pourquoi | Traitement retenu |
|---|---|---|
| **4** — cheval au galop | Animer une foulée déforme les pattes à coup sûr | Cheval **figé en pleine foulée**, seule la caméra bouge. Le galop se lit au montage, par la coupe rapide avec le plan 5 |
| **8** — musiciens qui entrent | Marche humaine = déformation des jambes | Figures **immobiles de dos**, caméra qui avance vers elles. On lit l'entrée en piste sans animer la marche |
| **7 / 9** — foules | Des centaines de petits visages qui morphent | Foule en **silhouette compacte**, aucun mouvement individuel prompté, seule la lumière vacille |

Si l'un de ces trois plans tremble malgré tout, la solution n'est pas de relancer : c'est de **garder l'image fixe** et de créer le mouvement au montage par un zoom lent. Personne ne verra la différence, et vous économisez 22,5 crédits.

---

## DURÉES — le point à vérifier en premier

Seedance produit des clips de **durée fixe** (5 ou 10 secondes selon le modèle et la résolution — **à confirmer sur le catalogue**). Vos plans font 6 à 11 secondes. Ils ne tomberont pas juste.

La méthode sûre : **générer au palier immédiatement supérieur, puis couper au montage.** Le coût est le même quelle que soit la portion gardée, et couper ne dégrade rien — contrairement à un ralenti, qui ferait ramer les hachures.

| # | Durée voulue | Générer | À couper |
|---|---|---|---|
| 1 | 6 s | 10 s | 4 s |
| 2 | 6 s | 10 s | 4 s |
| 3 | 7 s | 10 s | 3 s |
| 4 | 7 s | 10 s | 3 s |
| 5 | 6 s | 10 s | 4 s |
| 6 | 7 s | 10 s | 3 s |
| 7 | 7 s | 10 s | 3 s |
| 8 | 7 s | 10 s | 3 s |
| 9 | 7 s | 10 s | 3 s |
| 10 | 7 s | 10 s | 3 s |
| 11 | 8 s | 10 s | 2 s |
| 12 | 7 s | 10 s | 3 s |
| 13 | 11 s | 10 s + 1 s de gel | — |
| 14 | 11 s | réutiliser le clip 1, ralenti ou gel | — |

**Coupez toujours la fin, jamais le début.** La dérive d'un modèle vidéo s'accumule avec le temps : les deux dernières secondes sont les plus instables. Garder le début, c'est garder le plus propre.

Le plan 13 est le seul qui dépasse 10 secondes. Tenez la dernière frame en gel une seconde — l'acrobate suspendue immobile fonctionne, c'est même un beau temps mort avant la chute.

---

## LES 14 PROMPTS DE MOUVEMENT

À utiliser en **image-to-video** : l'image fixe correspondante en entrée, ce texte en prompt de mouvement. Modèle `seedance_2_0`, aspect `9:16`, résolution 4K.

Le bloc `NEGATIVE` est **identique partout** — c'est lui qui protège la gravure. Ne le modifiez pas et ne l'allégez pas.

> **NEGATIVE commun (à coller dans chaque prompt) :**
> no morphing, no warping, no melting, no flickering lines, no shimmering texture, no style drift, no added detail, no photorealism, no colour shift, no text, no captions, no watermark, no face deformation, preserve the etched line work and paper grain exactly.

---

**Plan 1 — la piste vide (ouverture)**
> MOTION: extremely slow push-in toward the centre of the ring, barely perceptible. The engraving itself is completely static. Only fine dust motes drift slowly through the air. Locked, steady, no rotation.

**Plan 2 — macro sciure**
> MOTION: very slow lateral drift across the sawdust, shallow focus breathing gently. The grains themselves do not move. Static engraving, camera drift only.

**Plan 3 — la silhouette dans la porte**
> MOTION: the officer stands perfectly still, absolutely no body movement. Straw dust and fine particles drift slowly downward through the shaft of light. Extremely slow push-in toward the doorway.

**Plan 4 — le cavalier (haut risque)**
> MOTION: the horse and rider are frozen mid-stride, a static engraved tableau — no leg movement, no gait animation whatsoever. Only the mane, the coat tails and airborne dust drift. Slow camera push-in from below.

**Plan 5 — les sabots**
> MOTION: clods of earth and dust hang and drift slowly upward in the air, as if in slow motion. The hooves themselves stay frozen. Camera locked low and still.

**Plan 6 — le fouet**
> MOTION: slow camera travel forward along the line of the whip, following it into depth toward the distant ring edge. The whip itself stays perfectly still on the ground. Fine sawdust drifts.

**Plan 7 — les galeries (haut risque)**
> MOTION: the crowd is a single static silhouette mass — no individual figures move, no heads turn. Only the gaslight glow pulses gently and haze drifts. Very slow tilt upward across the tiers.

**Plan 8 — les musiciens (haut risque)**
> MOTION: the figures are frozen mid-step from behind, no walking animation, no limb movement. Only the suspended dust in the light beams drifts. Slow camera push-in following behind them.

**Plan 9 — le Cirque Napoléon (haut risque)**
> MOTION: slow tilt upward across the stacked balconies. The crowd stays a static silhouette mass, no individual movement. Chandelier light flickers faintly, haze drifts in the upper air.

**Plan 10 — les mains sur la barre**
> MOTION: the hands stay locked in their grip, no finger movement. Fine chalk dust falls slowly from the bar. Extremely slow push-in on the knuckles.

**Plan 11 — le corps en vol** ⭐ le plan test
> MOTION: the body hangs suspended in the air in extreme slow motion, drifting almost imperceptibly, arms held still. The shaft of light breathes faintly. No limb articulation, no rotation. Slow, weightless, held.

**Plan 12 — le maillot**
> MOTION: slow overhead drift across the garment, raking light moving gently across the knit texture. The fabric is completely still, no rippling. Static engraving, camera move only.

**Plan 13 — l'acrobate sur tissus**
> MOTION: the silks ripple very slowly along their length. The acrobat's silhouette stays still, no limb movement, no spinning. Slow descending camera move. Single beam of light breathing faintly.

**Plan 14 — la piste vide (bouclage)**
> Réutiliser le clip du plan 1, **ralenti à environ 55 %** pour atteindre 11 secondes. Le bouclage exige un cadrage strictement identique — le regénérer produirait une variation, même minime, et casserait l'effet. Aucun crédit dépensé.

---

## LA 4K — ce qu'il faut savoir avant de payer pour elle

Vous demandez de la 4K, le dossier la prévoit. Un point à connaître avant de valider la dépense.

En 9:16, la 4K représente **2160 × 3840**. Or TikTok, Shorts et Reels **rediffusent en 1080 × 1920** : ils rééencodent et redimensionnent systématiquement à la publication. Les pixels supplémentaires ne parviennent pas au spectateur.

La 4K garde deux usages réels, et si l'un des deux vous intéresse elle est justifiée :

- **de la marge de recadrage** — recadrer, stabiliser ou repositionner un plan sans perte ;
- **un master pérenne** — un fichier source de qualité pour un remontage ou une republication ultérieure.

Sur un film composé de gravures fixes légèrement animées, la 4K n'apporte en revanche **aucun gain de netteté perceptible** : la finesse vient du trait de la lithographie, déjà contenu dans l'image 2k source. Agrandir ne crée pas de détail.

**Mon conseil :** générez en **1080p vertical** si le budget compte, et réservez la 4K aux plans 1, 11 et 14 — l'ouverture, le plan clé et le bouclage. Vous gardez le master là où il sert et vous économisez sur les onze autres.

Si vous voulez la 4K partout, c'est votre choix et le dossier est prêt pour ça : passez simplement `resolution: 4k` sur les quatorze appels et revoyez le budget en conséquence.

---

## ORDRE DE PRODUCTION

1. **Image fixe du plan 11** — 2 crédits. Validez le style gravure.
2. **Animation du plan 11** — ~22,5 crédits. Validez la tenue sous mouvement. **Point de décision.**
3. **Images fixes 3 et 9** — 4 crédits. Les deux autres cas difficiles.
4. **Animations 3 et 9** — ~45 crédits. Ce sont les plans à foule, les plus risqués.
5. **Les 10 images restantes** — 20 crédits.
6. **Les animations restantes, par groupes de quatre** — contrôle à chaque groupe.
7. **Voix off** — `seed_audio`, script dans `cirque-90s.md`.
8. **Montage** — assemblage, coupes selon le tableau des durées, incrustation de `13-metres.srt`.

Ne lancez jamais les quatorze animations d'un bloc. À 22,5 crédits pièce, un défaut systématique découvert au douzième plan coûte 270 crédits.

---

## MONTAGE

- **Coupes franches**, aucune transition. Le film tient par le rythme, pas par les fondus.
- **Couper la fin des clips**, jamais le début — la dérive s'accumule.
- **Voix off d'abord**, images calées dessus ensuite. Le minutage de `cirque-90s.md` suit la voix.
- **Sous-titres incrustés** sur 100 % de la durée, fichier `13-metres.srt` (règle 6).
- **Plans 1 et 14 rigoureusement identiques** — c'est le bouclage qui déclenche le replay (règle 7).
- **Trois effets sonores** : sabots au galop, brouhaha de foule, cloche de cirque sur le logo final.

---

## À CONFIRMER SUR LE CATALOGUE EN DIRECT

Je n'ai pas accès à Higgsfield. Vérifiez ces quatre points avant de lancer :

1. **Le coût réel de `seedance_2_0`** en 9:16 4K — mon estimation à 22,5 crédits date d'une lecture antérieure et peut avoir changé.
2. **Les durées de clip disponibles** — 5 s, 10 s, ou autre chose. Tout le tableau des coupes en dépend.
3. **La 4K est-elle native** ou faut-il un `upscale_video` séparé, avec son propre coût.
4. **Le mode image-to-video** est bien celui qui accepte une image en première frame, et non un simple guidage de style.

Dites-moi ce que vous lisez et je réajuste le dossier — c'est du calcul, je le refais en deux minutes.
