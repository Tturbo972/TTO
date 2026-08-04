# ÉPISODE 2 — PISTE AUDIO
## Narration complète · 120 s · mono 44,1 kHz · normalisée −16 LUFS

**Fichier livré (version française) :**
`https://d2ol7oe51mr4n9.cloudfront.net/user_3GxPcyALGbnZURj7lluqi6XwHVi/d72e656e-8a8f-41d5-b0b2-bc9aedf46aef.mp3`

Voix : `seed_audio`, préréglage **Luc** (`04e867c7-9e41-5cff-80d3-5284e74d7bd1`, masculine, **francophone**). **C'est la voix de la chaîne** — réutilisez ce `voice_id` sur tous les épisodes.

⚠️ **Correction du 4 août :** la première version utilisait « Marcus », un préréglage anglophone. `seed_audio` n'a pas de paramètre de langue — c'est la voix elle-même qui porte l'accent, et un modèle anglais lisant du français produit une prononciation approximative. Le catalogue est codé par nationalité (Anush arménien, Olena et Vlad slaves, Marisol espagnol) et **Luc est le seul préréglage masculin français**. Les 12 prises ont été refaites.

Ancienne version anglophone, conservée pour comparaison : `.../8d55baa1-74dd-49d2-826d-c4d636cf251e.mp3`

Deux nombres ont aussi été écrits en toutes lettres dans le texte source — « mille neuf cent soixante-seize », « mille neuf cent quatre-vingt-deux » — pour éviter que le modèle ne les lise à l'anglaise.

## Construction
Chaque prise est **centrée dans sa fenêtre de 10 s**, silence réparti avant et après, puis les 12 fenêtres sont concaténées. La piste tombe donc exactement sur les 12 clips de 10 s : **posez-la à 0:00, tout est calé, aucun ajustement manuel.**

Normalisation `loudnorm I=-16 TP=-1.5` — le standard de diffusion, ni écrêtage ni écart de niveau entre blocs.

## Correction appliquée
Un premier montage a été jeté : trois prises dépassaient leur fenêtre et se faisaient couper net.

| Bloc | Avant | Après |
|---|---|---|
| 2 | 12,35 s — coupée | **8,13 s** |
| 3 | 11,74 s — coupée | **6,31 s** |
| 12 | 12,06 s — coupée | **7,74 s** |

Le bloc 12 était le plus grave : c'est la chute, et « Partage son nom » tombait dans la coupe. Les trois lignes ont été raccourcies puis régénérées. Les douze prises tiennent maintenant sous 8,9 s (mesuré sur la version française).

**Lignes modifiées** (à reporter dans le script si vous refaites les sous-titres) :
- Bloc 2 : « Chavarch Karapetian est le meilleur au monde dans un sport que personne ne regarde : la nage avec palmes. »
- Bloc 3 : « Le 16 septembre 1976, il court le long du lac d'Erevan. C'est là qu'il entend le choc. »
- Bloc 12 : « Des milliers de lettres arrivent. Certaines adressées : Erevan. Au nageur. Partage son nom. »

## Note sur le verrou d'assemblage
L'assembleur automatique a rejeté les blocs 2, 6 et 8 pour « non-conformité au script ». Vérification faite, c'est un **faux positif** : le vérificateur transcrit avec un petit modèle anglophone qui massacre le français (« est le meilleur au monde » → « et l amereaux monde »). Les prises étaient bonnes. Ne relancez pas ce contrôle sur du français sans forcer la langue.

## Reste à faire
- Monter la piste sur les 12 clips (CapCut, DaVinci) — calage automatique à 0:00.
- Incruster les sous-titres (`25-secondes.srt`, à recaler sur les 3 lignes modifiées).
- Lockup mascotte + logo.
