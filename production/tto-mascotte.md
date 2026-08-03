# TTO — LA MASCOTTE
## Personnage récurrent de chaîne · brief de production

À décider **avant la publication de l'épisode 1**. La règle 10 gèle le hook après la première mise en ligne, et la mascotte en fait partie : elle ne pourra plus changer sans casser l'effet de reconnaissance.

---

## LA CONTRAINTE À RÉSOUDRE

La règle 9 impose le faceless intégral : silhouettes, mains, contre-jour, **aucun visage identifiable**. Une mascotte classique — un personnage avec des yeux, une bouche, des expressions — la violerait frontalement.

La solution n'est pas d'assouplir la règle. C'est de choisir un personnage **dont l'absence de visage est le principe même**, pas une amputation. Un personnage qu'on reconnaît à sa silhouette et à son geste, jamais à ses traits.

C'est aussi ce qui protège la chaîne sur le fond : un visage généré qui reviendrait à chaque épisode finirait par ressembler à quelqu'un de réel. Une silhouette, non.

---

## CONCEPT RETENU — « L'ARPENTEUR »

Une silhouette en contre-jour, manteau long, chapeau à large bord, tenant **un compas d'épaisseur** — l'instrument de mesure du graveur et du cartographe.

### Pourquoi celui-là

**Le compas est littéralement le sujet de la chaîne.** TTO parle du détail qui n'a jamais changé. Or le compas à pointes sèches est identique dans les gravures du XVIe siècle et dans un atelier d'aujourd'hui. L'outil qui mesure les constantes est lui-même une constante. La mascotte *est* la thèse de la chaîne, elle ne l'illustre pas.

**Il rime avec l'épisode 1.** Les treize mètres sont un rayon — la portée d'un fouet depuis le centre. Astley a tracé un cercle exactement comme un compas en trace un. Le lien est structurel, pas décoratif.

**Il tient au format vignette.** Manteau long, chapeau, un bras tendu tenant un objet pointu : la silhouette est lisible à 100 pixels de côté. C'est le vrai test d'une mascotte, et beaucoup échouent là.

**Il est faceless par construction.** En contre-jour intégral, la question du visage ne se pose jamais. Aucun risque de ressemblance avec une personne réelle.

**Il est intemporel.** Le costume évoque le XVIIIe–XIXe sans se dater précisément. Il fonctionnera pour un épisode sur les rails romains comme sur les touches de piano.

---

## DEUX MODES D'USAGE — le choix qui compte vraiment

C'est ici que se joue le coût et le risque, bien plus que dans le dessin lui-même.

### Mode A — emblème fixe **(recommandé)**

La mascotte est **une image unique, générée une seule fois, réutilisée telle quelle à vie**. Exactement comme le logo.

- **Coût total : 2 crédits. Une fois. Pour toujours.**
- **Dérive : impossible.** C'est le même fichier à chaque épisode.
- Elle apparaît dans le lockup final du hook, en position fixe.

### Mode B — personnage récurrent en situation

La mascotte apparaît dans chaque épisode **en interaction avec le sujet** : elle mesure un rail, une touche de piano, une piste de cirque.

- **Coût : ~2 crédits par épisode**, plus les ratés.
- **Dérive garantie à terme.** Même avec une image de référence passée à chaque génération, la silhouette bouge : le chapeau change de bord, le manteau de longueur, la carrure de proportion. Sur dix épisodes, ce n'est plus le même personnage.
- Demande une fiche de référence et un contrôle à chaque épisode.

### Mon conseil, franchement : le mode A

Le mode B est séduisant sur le papier et c'est là que les chaînes perdent leur cohérence. Un emblème fixe qui revient à l'identique **crée plus de reconnaissance** qu'un personnage qui varie légèrement à chaque fois — la variation, même petite, casse précisément ce que le rituel construit.

Et le raisonnement est déjà dans votre charte : le hook fonctionne « par la répétition stricte ». La mascotte suit la même loi.

Le mode A coûte 2 crédits une fois. Le mode B coûte 2 crédits par épisode et vous met un contrôle qualité sur les bras à chaque fois, pour un gain nul.

---

## LE PROMPT — mode A

Modèle `nano_banana_pro` · **1:1** · 2k · 2 crédits.

Format carré pour la même raison que le logo : il se recadre vers le 9:16 comme vers le 16:9 sans perte.

> A 19th-century lithographic engraving, square emblem composition: the full-length silhouette of a lone figure in a long coat and wide-brimmed hat, seen in complete backlit silhouette with absolutely no facial features visible, standing in profile and holding up a pair of brass dividers in one hand as if measuring something distant. Centred, symmetrical, generous clean margins, strong readable silhouette against a plain luminous background. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No face, no eyes, no facial detail, no text, no captions, no watermark.

### Contrôle avant adoption

Trois défauts disqualifient le résultat, régénérez sans hésiter :

1. **Un visage apparaît** — même esquissé, même de profil. Le contre-jour doit être total.
2. **Le compas est illisible** ou ressemble à autre chose (une arme, un bâton). C'est l'élément porteur de sens, il doit se lire.
3. **La silhouette ne tient pas en petit.** Réduisez l'image à 100 pixels : si vous ne reconnaissez plus ni le chapeau ni le bras tendu, elle est trop détaillée.

Le test de la vignette est le plus important des trois. Une mascotte se voit d'abord en miniature.

---

## PLACEMENT DANS LE HOOK

La mascotte rejoint le **temps ⑥**, celui de la cloche et du logo. Elle ne crée pas de nouveau temps et **n'allonge pas le hook d'une seule image**.

```
⑥ 0:12 → 0:13 · CLOCHE + LOCKUP
   Plein écran, ~1 seconde :
   la silhouette de l'Arpenteur, le logo TTO dessous.
   La cloche sonne exactement sur l'apparition.
   Puis coupe directe sur le plan 1 de l'épisode.
```

Deux raisons de la mettre là plutôt qu'ailleurs.

**Pas au temps ①.** La charte est explicite : à l'ouverture, « l'image ne doit pas concurrencer la phrase ». Une mascotte à cet endroit détournerait l'attention de la phrase choc, qui est le moment le plus important du film.

**Au temps ⑥, elle profite d'un rituel déjà construit.** La cloche, le logo et le plein écran d'une seconde existent déjà. La mascotte s'y ajoute sans rien coûter en durée ni en attention — elle densifie la signature au lieu d'en créer une seconde.

### Le lockup

Générez la mascotte et le logo **séparément**, puis assemblez-les au montage. Ne les générez jamais ensemble dans une seule image : les modèles ratent régulièrement les lettres, et vous seriez obligé de refaire la mascotte à chaque tentative ratée sur le « TTO ».

Composition : silhouette centrée dans le tiers supérieur, logo centré dessous, fond papier ancien commun. Un fichier PNG monté une fois, réutilisé à vie.

---

## VARIANTE — « LA MAIN ET LE COMPAS »

Si l'Arpenteur vous paraît trop figuratif, voici la version dépouillée : **pas de personnage du tout**, seulement une main tenant le compas.

> A 19th-century lithographic engraving, square emblem composition: a single hand holding a pair of brass dividers open above a plain surface, seen from a slightly raised angle, the points of the dividers resting precisely on the surface. No arm beyond the wrist, no figure, no person. Centred, symmetrical, generous clean margins. Etched line work and dense cross-hatching, aged paper texture with visible fibre and foxing, limited palette of ink black, warm sepia and a single crimson accent, subtle paper grain. No text, no captions, no watermark.

**Ce qu'elle gagne :** conformité absolue à la règle 9 — une main est déjà citée dans la charte comme motif autorisé. Aucun risque de ressemblance. Plus abstraite, plus sobre, elle vieillira très bien.

**Ce qu'elle perd :** moins de présence, moins mémorisable. Une main se distingue moins qu'une silhouette à chapeau, surtout en vignette.

**Départage :** générez les deux, 4 crédits, et réduisez-les à 100 pixels côte à côte. Celle que vous reconnaissez encore gagne. C'est le seul test qui compte.

---

## SI VOUS CHOISISSEZ QUAND MÊME LE MODE B

Il vous faut alors une **fiche de référence** — une planche unique montrant le personnage sous plusieurs angles, qui servira d'image de référence à chaque génération ultérieure.

> A 19th-century lithographic engraving, character reference sheet: the same silhouetted figure in a long coat and wide-brimmed hat shown three times side by side against a plain background — front view, side profile, and three-quarter view — each in complete backlit silhouette with no facial features whatsoever, holding a pair of brass dividers. Consistent proportions across all three, evenly spaced, plain background, clean margins. Etched line work and cross-hatching, aged paper texture, ink black and warm sepia. No face, no eyes, no text, no captions, no watermark.

Ensuite, passez cette planche en image de référence sur **chaque** génération de la mascotte en situation, et vérifiez à chaque épisode que le chapeau, la longueur du manteau et la carrure n'ont pas bougé.

Higgsfield dispose d'un workflow dédié aux fiches de personnage — appelez `get_workflow_instructions` avec `{ workflow: "character-sheet" }` avant de générer, il contient les gabarits à jour. Je n'ai pas pu le consulter, l'accès m'étant fermé ; le prompt ci-dessus est écrit d'après les principes du genre et sera moins bon que le gabarit officiel. Utilisez le leur s'il est disponible.

---

## RÈGLES D'USAGE

- **Générer une seule fois. Ne jamais régénérer.** Conservez le fichier source, sauvegardez-le hors du conteneur.
- **Toujours à la même place**, à la même taille, à la même durée. Comme le logo.
- **Jamais en filigrane** pendant l'épisode, jamais en incrustation permanente.
- **Ne l'animez pas.** Elle apparaît en coupe franche, une seconde, fixe. Une mascotte animée à chaque épisode réintroduit exactement la dérive que le mode A élimine.
- **Elle n'a pas de nom à l'écran.** « L'Arpenteur » est un nom de travail, interne. Le nommer dans une vidéo l'obligerait à devenir un personnage avec une histoire, ce qu'il n'est pas.

---

## CE QU'IL RESTE À DÉCIDER

1. **Arpenteur ou Main au compas** — départagez par le test de la vignette, 4 crédits.
2. **Mode A ou mode B** — mon conseil est le mode A, sans réserve.
3. **Le lockup** — mascotte au-dessus du logo, ou côte à côte. À trancher en voyant les deux images.

Une fois ces trois points fixés et l'épisode 1 publié, la mascotte est gelée pour toute la chaîne.
