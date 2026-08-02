# TTO

Chaîne YouTube/TikTok faceless de récits courts.

**Concept :** *le détail qui n'a jamais changé.* Chaque épisode part d'une mesure ou d'un objet concret et vérifiable, puis en déroule l'histoire jusqu'à un renversement.

**Gabarit de titre :** `[CHIFFRE] — [le détail que personne ne remarque]`

---

## Contenu du dépôt

| Fichier | Rôle |
|---|---|
| `production/tto-charte-hook.md` | **Charte du hook** — gabarit d'ouverture fixe, identique à chaque épisode. Inclut le brief du logo. À lire en premier. |
| `production/cirque-90s.md` | **Épisode 1 — « 13 mètres »**, version 1:30. Script, shot list, 12 prompts prêts à coller. C'est la version de référence. |
| `production/cirque-production.md` | Version 3:05 du même épisode. Conservée pour référence, remplacée par la version 1:30. |
| `production/prompts-24-pret-a-coller.md` | Les 24 prompts de la version longue. |
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
9. **Faceless intégral** — silhouettes, mains, contre-jour. Aucun visage identifiable.
10. **Le hook ne change jamais** une fois le premier épisode publié.

---

## Pile technique

- **Images :** Higgsfield, `nano_banana_pro` (résout vers `nano_banana_2`), 16:9, 2k — 2 crédits/image.
- **Voix off :** Higgsfield, `seed_audio`.
- **Vidéo générée :** écartée. `seedance_2_0` coûte 22,5 crédits/plan contre 2 pour une image, et la gravure au trait se dégrade en vidéo générée. Le mouvement se fait au montage.

`.claude/settings.json` autorise les outils Higgsfield nécessaires. `generate_video` en est **volontairement exclu** — c'est le poste coûteux, il doit rester un geste délibéré.

---

## État

- Épisode 1 : script, hook et prompts finalisés.
- Plan 1 généré. **Direction artistique non validée visuellement.**
- Reste à produire : 11 plans, le logo, la voix off, les 3 effets sonores.
