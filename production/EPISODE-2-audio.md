# ÉPISODE 2 — PISTE AUDIO
## Narration complète · 120 s · mono 44,1 kHz · normalisée −16 LUFS

**Fichier livré :**
`https://d2ol7oe51mr4n9.cloudfront.net/user_3GxPcyALGbnZURj7lluqi6XwHVi/8d55baa1-74dd-49d2-826d-c4d636cf251e.mp3`

Voix : `seed_audio`, préréglage **Marcus** (`6f98d3dd-324f-4845-8c28-c1d1647a06cd`, masculine). **C'est désormais la voix de la chaîne** — réutilisez ce `voice_id` sur tous les épisodes.

## Construction
Chaque prise est **centrée dans sa fenêtre de 10 s**, silence réparti avant et après, puis les 12 fenêtres sont concaténées. La piste tombe donc exactement sur les 12 clips de 10 s : **posez-la à 0:00, tout est calé, aucun ajustement manuel.**

Normalisation `loudnorm I=-16 TP=-1.5` — le standard de diffusion, ni écrêtage ni écart de niveau entre blocs.

## Correction appliquée
Un premier montage a été jeté : trois prises dépassaient leur fenêtre et se faisaient couper net.

| Bloc | Avant | Après |
|---|---|---|
| 2 | 12,35 s — coupée | **6,75 s** |
| 3 | 11,74 s — coupée | **7,99 s** |
| 12 | 12,06 s — coupée | **8,79 s** |

Le bloc 12 était le plus grave : c'est la chute, et « Partage son nom » tombait dans la coupe. Les trois lignes ont été raccourcies puis régénérées. Les douze prises tiennent maintenant sous 8,8 s.

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
