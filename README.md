# TTO

Chaîne YouTube/TikTok faceless de récits courts.

**Concept :** *le détail qui n'a jamais changé.* Chaque épisode part d'une mesure ou d'un objet concret et vérifiable, puis en déroule l'histoire jusqu'à un renversement.

**Gabarit de titre :** `[CHIFFRE] — [le détail que personne ne remarque]`

---

## Contenu du dépôt

| Fichier | Rôle |
|---|---|
| `production/EPISODE-1-5MIN.md` | **⭐ Épisode 1, version 5 minutes** — script, 30 plans, prompts, plan d'animation hybride. Version de référence. |
| `production/EPISODE-1-youtube-kit.md` | **Kit YouTube** — titre, vignettes, description, chapitres, écran de fin, checklist. |
| `production/13-metres-5min.srt` | Sous-titres de la version 5 min, 142 segments. |
| `production/EPISODE-1-feuille-de-prod.md` | **⭐ Feuille de production épisode 1** — tous les prompts dans l'ordre d'exécution, avec cases à cocher et coûts. C'est le document à ouvrir pour produire. |
| `production/tto-charte-hook.md` | **Charte du hook** — gabarit d'ouverture fixe, identique à chaque épisode. Inclut le brief du logo. À lire en premier. |
| `production/cirque-90s.md` | **Épisode 1 — « 13 mètres »**, 1:44 en **9:16 vertical**. Script, shot list, 13 prompts recomposés pour le vertical. C'est la version de référence. |
| `production/tto-mascotte.md` | **La mascotte TTO** — concept, prompt, placement dans le hook. À geler avant publication de l'épisode 1. |
| `production/seedance-animation.md` | **Dossier d'animation Seedance** — 14 prompts de mouvement, budget, gestion des durées, stratégie 4K. |
| `production/13-metres.srt` | Sous-titres de l'épisode 1, 49 segments calés sur le minutage. |
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
- **Voix off :** Higgsfield, `seed_audio`.
- **Animation :** `seedance_2_0` en image-to-video, 9:16, ~22,5 crédits/plan. Chaque image fixe validée sert de première frame. Voir `production/seedance-animation.md` — le mouvement vient de la caméra, jamais du sujet, pour protéger la gravure.

`.claude/settings.json` autorise les outils Higgsfield, `generate_video` compris depuis le passage à l'animation. C'est le poste coûteux — voir le budget par paliers dans le dossier Seedance avant de lancer une série.

---

## État

- Épisode 1 : script, hook, prompts 9:16 et sous-titres finalisés.
- Plan 1 généré en 16:9 — **à refaire en 9:16**. Direction artistique non validée visuellement.
- Reste à produire : 13 images (26 crédits), 13 animations (~292 crédits), le logo, la voix off, les 3 effets sonores.
- **Accès Higgsfield fermé depuis cet environnement** : les 5 domaines sont refusés par la politique réseau. La production se fait dans l'application.
