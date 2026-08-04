# TTO

Chaîne YouTube/TikTok faceless de récits courts.

**Concept :** *le détail qui n'a jamais changé.* Chaque épisode part d'une mesure ou d'un objet concret et vérifiable, puis en déroule l'histoire jusqu'à un renversement.

**Gabarit de titre :** `[CHIFFRE] — [le détail que personne ne remarque]`

---

## Contenu du dépôt

| Fichier | Rôle |
|---|---|
| `production/EPISODE-1-5MIN.md` | **⭐ Épisode 1, version 5 minutes** — script, 30 plans, prompts, plan d'animation hybride. Version de référence. |
| `production/EPISODE-1-youtube-kit.md` | **Kit YouTube ép. 1** (long-form 5:12) — titre, vignettes, description, chapitres, checklist. |
| `production/EPISODE-1-tiktok-kit.md` | **Kit TikTok ép. 1** — couverture, légende, label IA, stratégie 3 parties. |
| `production/EPISODE-2-25-secondes.md` | **Épisode 2 « 25 secondes »** — analyse maratrium, script 2:18, production exécutée. |
| `production/EPISODE-2-assets.md` | Les 24 assets générés de l'épisode 2 (12 images + 12 clips). |
| `production/EPISODE-2-youtube-kit.md` | **Kit YouTube ép. 2** — c'est un **Short** : première frame, titre, description, checklist. |
| `production/25-secondes.srt` | Sous-titres épisode 2, 63 segments. |
| `production/EPISODE-2-audio.md` | **Piste audio ép. 2** — 120 s, voix Marcus, calée sur les 12 clips. |
| `production/prompts-a-coller.txt` | Prompts d'**images** en texte brut, prêts à coller. |
| `production/prompts-animation-a-coller.txt` | Prompts d'**animation** Seedance en texte brut, 29 clips. |
| `production/13-metres-5min.srt` | Sous-titres de la version 5 min, 142 segments. |
| `production/EPISODE-1-feuille-de-prod.md` | **⭐ Feuille de production épisode 1** — tous les prompts dans l'ordre d'exécution, avec cases à cocher et coûts. C'est le document à ouvrir pour produire. |
| `production/tto-charte-hook.md` | **Charte du hook** — gabarit d'ouverture fixe, identique à chaque épisode. Inclut le brief du logo. À lire en premier. |
| `production/cirque-90s.md` | Version 2:00 en 9:16. Archive, remplacée par la version 5 minutes. |
| `production/tto-mascotte.md` | **La mascotte TTO** — concept, prompt, placement dans le hook. À geler avant publication de l'épisode 1. |
| `production/seedance-animation.md` | **Dossier d'animation Seedance** — 14 prompts de mouvement, budget, gestion des durées, stratégie 4K. |
| `production/13-metres.srt` | Sous-titres de la version 2:00. Archive. |
| `production/cirque-production.md` | Version 3:05 en 16:9. Archive, remplacée. |
| `production/prompts-24-pret-a-coller.md` | Les 24 prompts de la version longue, en 16:9. Archive. |
| `production/lustig-production.md` | Sujet alternatif (Victor Lustig / Tour Eiffel), non produit. |

---

## Règles de production

Les règles éditoriales et de production sont détaillées dans les dossiers. En résumé :

1. **Ancre familière avant le fait nouveau** — la surprise vient après la reconnaissance.
2. **Un seul arc**, aucune digression.
3. **Récit au présent.**
4. Sources et disclaimer IA **en description**, jamais dans la voix off.
5. **Erratum public** en cas d'erreur — on corrige en clair, on ne supprime pas.
6. **Sous-titres incrustés** sur 100 % de la durée.
7. **Le dernier plan rejoue le premier** — c'est le bouclage qui déclenche le replay.
8. **Direction artistique verrouillée** : gravure lithographique XIXe, bloc de prompt identique sur tous les plans et tous les épisodes.
9. **Faceless intégral** — silhouettes, mains, contre-jour. Aucun visage identifiable. La mascotte elle-même est une silhouette en contre-jour : sans visage par construction, pas par retouche.
10. **Le hook ne change jamais** une fois le premier épisode publié.

---

## Pile technique

- **Images :** Higgsfield, `nano_banana_pro`, **9:16 vertical**, 2k — 2 crédits/image.
- **Voix off :** Higgsfield, `seed_audio`, préréglage **Marcus** (`6f98d3dd-324f-4845-8c28-c1d1647a06cd`) — voix de chaîne, à réutiliser sur tous les épisodes.
- **Animation :** `kling3_0_turbo` en image-to-video, 9:16, 720p, 15 crédits/clip de 10 s. L'offre illimitée n'existe pas sur ce compte et Seedance 2.0 coûte 90 à 220 crédits le clip — hors budget. Le mouvement vient de la caméra, jamais du sujet, pour protéger la gravure.

`.claude/settings.json` autorise les outils Higgsfield, `generate_video` compris depuis le passage à l'animation. C'est le poste coûteux — voir le budget par paliers dans le dossier Seedance avant de lancer une série.

---

## État (4 août 2026)

- **Épisode 2 « 25 secondes » : plans produits.** 12 images + 12 clips animés, tous réussis (204 crédits). Manifeste dans `EPISODE-2-assets.md`. Reste : voix off (choix de voix à faire), montage, lockup.
- Épisode 1 « 13 mètres » : dossier complet (script 5:12, 30 plans, prompts, sous-titres, kits YouTube et TikTok). Images non générées, sauf le plan 24 (image + clip test).
- Mascotte et logo : prompts prêts, non générés (6 crédits, une fois).
- **Solde : 88,5 crédits.**
- L'accès Higgsfield fonctionne depuis la session via les outils MCP (serveur « Magic »). Le CLI et les domaines directs restent bloqués par la politique réseau.
