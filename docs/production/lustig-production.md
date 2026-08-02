# L'HOMME QUI A VENDU LA TOUR EIFFEL
## Dossier de production — vidéo 3 minutes, faceless YouTube, Seedance 2.0 / 1080p

---

## PARAMÈTRES TECHNIQUES

| Paramètre | Valeur | Note |
|---|---|---|
| Modèle | `seedance_2_0` | demandé |
| Résolution | 1080p | demandé |
| Format | **16:9** (1920×1080) | YouTube long — voir note format |
| Durée totale | ~3:05 | 185 s |
| Nombre de plans | 24 | ~7,5 s moyen |
| Voix off | `seed_audio` (Seed Audio 1.0) | voix masculine FR, débit posé |
| Sous-titres | incrustés, 100 % de la durée | |

### Note format — à trancher
La chaîne de référence (@maratrium) publie en **9:16 / ~60 s**. Vous demandez **3 min sur YouTube faceless**, ce qui implique **16:9**. Ce n'est pas le même format : la structure ci-dessous est réécrite pour la durée longue (4 actes + chute) au lieu de l'arc unique de 60 s. Si vous vouliez en réalité un Short vertical, dites-le : il faut alors couper à l'acte 3 uniquement.

### Note coût — non vérifiée
Je n'ai pas pu interroger `balance` ni les contraintes de durée de `seedance_2_0`. **24 générations en 1080p représentent un volume de crédits significatif.** Avant de lancer la série complète, faites un `get_cost: true` sur un plan test pour connaître le coût unitaire, puis multipliez par 24.

---

## DIRECTION ARTISTIQUE — bloc à coller dans CHAQUE prompt

> `cinematic 1920s-1940s period piece, desaturated warm sepia and teal palette,
> 35mm film grain, soft volumetric light, shallow depth of field, subtle haze,
> muted contrast, no text, no captions, no watermark, 16:9`

**Règle absolue :** ce bloc est identique sur les 24 plans. C'est lui qui crée la signature visuelle de la chaîne. Ne jamais le faire varier d'une vidéo à l'autre.

**Contrainte visages :** aucun plan ne montre un visage identifiable en gros plan frontal net. Silhouettes, dos, mains, contre-jour, profils flous. Cela évite les problèmes de ressemblance avec des personnes réelles et renforce l'esthétique.

---

## SCRIPT VOIX OFF (~480 mots)

### HOOK — 0:00 → 0:14
> En 1925, un homme entre dans un hôtel parisien avec de faux papiers du gouvernement.
> Il en ressort avec l'équivalent d'un million d'euros.
> Il vient de vendre la Tour Eiffel.
> Et dans quelques mois, il reviendra la vendre une deuxième fois.

### ACTE 1 — L'homme — 0:14 → 0:48
> Il s'appelle Victor Lustig. Né en Bohême en 1890. Il parle cinq langues, porte des costumes sur mesure, et la police de trois continents lui connaît quarante-cinq identités différentes.
> Sa première fortune, il la fait avec une boîte en acajou. Une machine à imprimer les billets, dit-il. Il en glisse deux vrais à l'intérieur, la fait fonctionner devant l'acheteur — six heures pour produire un billet, explique-t-il — et repart avec des dizaines de milliers de dollars.
> Le temps que la victime comprenne, Lustig a traversé l'Atlantique.

### ACTE 2 — Capone — 0:48 → 1:22
> En 1930, il tente quelque chose que personne de sensé n'oserait. Il demande un rendez-vous à Al Capone.
> Il lui propose de doubler cinquante mille dollars en deux mois. Capone accepte.
> Lustig met l'argent dans un coffre. Et ne fait absolument rien.
> Deux mois plus tard, il revient, l'air défait, et rend la somme entière. L'opération a échoué, dit-il. Je suis désolé.
> Capone, touché par une honnêteté aussi rare dans son monde, lui donne cinq mille dollars de dédommagement.
> C'était exactement le plan depuis le début.

### ACTE 3 — La Tour — 1:22 → 2:24
> Mais son chef-d'œuvre, c'est Paris, 1925.
> Il lit un article dans le journal : la Tour Eiffel rouille. Elle devait être démontée en 1909. Elle est toujours là, et son entretien coûte une fortune à la ville.
> Lustig fait imprimer du papier à en-tête du ministère des Postes et Télégraphes. Il convoque cinq des plus gros ferrailleurs de France dans une suite d'hôtel. Il se présente comme directeur général adjoint.
> Le dossier est confidentiel : l'État a décidé de démolir la Tour. Sept mille tonnes de fer à vendre. Et la discrétion est impérative — le public ne doit rien savoir.
> Parmi les cinq, un homme veut ce contrat plus que les autres : André Poisson. Riche, mais tenu à l'écart des grands marchés parisiens. Lustig voit la faille.
> Alors il fait la chose la plus contre-intuitive de toute l'histoire de l'escroquerie : il réclame un pot-de-vin.
> Et ça marche. Parce qu'un fonctionnaire corrompu, en 1925, c'est parfaitement crédible.
> Poisson paie le pot-de-vin. Puis il paie la Tour Eiffel.
> Lustig prend le train pour Vienne avec une valise pleine de billets. Il attend le scandale dans les journaux. Il n'arrive jamais.
> Poisson est trop humilié pour porter plainte.

### ACTE 4 — La chute — 2:24 → 2:56
> Alors Lustig fait la seule chose logique : il revient à Paris. Et il recommence, avec un nouveau groupe de ferrailleurs.
> Cette fois, la victime prévient la police. Il s'échappe de justesse.
> Il finit par tomber en 1935, aux États-Unis, pour une affaire de fausse monnaie. Trahi par une maîtresse.
> Avant son procès, il s'évade en plein jour, le long d'une corde de draps, en faisant semblant de laver les vitres devant des dizaines de témoins.
> On le rattrape vingt-sept jours plus tard. Vingt ans à Alcatraz. Il y meurt d'une pneumonie en 1947.

### CHUTE — 2:56 → 3:05
> Sur son certificat de décès, à la ligne « profession », un employé avait écrit : apprenti vendeur.
> Et toi, tu la connaissais, cette histoire ?

---

## SHOT LIST — 24 plans Seedance 2.0

Chaque prompt = description ci-dessous **+ bloc de direction artistique**.

| # | Time | Durée | Prompt Seedance (à compléter avec le bloc DA) | Texte écran |
|---|---|---|---|---|
| 1 | 0:00 | 6 s | Wide shot of the Eiffel Tower under heavy grey sky, slow push-in, empty Paris street 1925 | **IL A VENDU LA TOUR EIFFEL** |
| 2 | 0:06 | 4 s | Gloved hands placing forged government letterhead documents on a marble desk, top-down, slow drift | |
| 3 | 0:10 | 4 s | Leather suitcase snapping shut over stacks of 1920s banknotes, low angle | |
| 4 | 0:14 | 7 s | Silhouette of an elegant man in a three-piece suit adjusting his cuffs before a hotel mirror, backlit, face not visible | **VICTOR LUSTIG** |
| 5 | 0:21 | 7 s | Slow pan across a row of forged passports and identity papers spread on dark wood | *45 identités* |
| 6 | 0:28 | 7 s | Ornate mahogany box with brass rollers on a table, warm lamplight, slow orbit | |
| 7 | 0:35 | 7 s | Close-up of a banknote slowly emerging from a brass slot, mechanical rollers turning | |
| 8 | 0:42 | 6 s | Ocean liner departing a harbour at dusk, wide shot, smoke trailing | |
| 9 | 0:48 | 7 s | Dark 1930s Chicago speakeasy interior, cigar smoke in a shaft of light, two silhouettes at a table | **1930 — CHICAGO** |
| 10 | 0:55 | 7 s | Hands sliding a thick envelope of cash across a table toward a heavy iron safe | |
| 11 | 1:02 | 7 s | Heavy safe door slowly closing, deep shadow, single light source | |
| 12 | 1:09 | 7 s | Calendar pages turning rapidly on a wall, dust motes in light | *2 mois plus tard* |
| 13 | 1:16 | 6 s | Hands pushing a small stack of banknotes back across the same table, reluctant gesture | **5 000 $ DE DÉDOMMAGEMENT** |
| 14 | 1:22 | 7 s | Newspaper page in close-up, 1925 French typography, headline about the Eiffel Tower, hands unfolding it | |
| 15 | 1:29 | 7 s | Macro shot of rusted iron rivets and flaking paint on a massive metal beam, slow tilt up | *« L'entretien coûte trop cher »* |
| 16 | 1:36 | 7 s | Letterpress printing official ministry letterhead, ink and paper, mechanical motion | **MINISTÈRE DES POSTES ET TÉLÉGRAPHES** |
| 17 | 1:43 | 8 s | Opulent 1920s hotel suite, five men in suits seated around a table seen from behind, chandelier light | |
| 18 | 1:51 | 7 s | One man leaning forward slightly more than the others, shot from behind, shallow focus | **ANDRÉ POISSON** |
| 19 | 1:58 | 7 s | Hands exchanging a discreet envelope beneath a table, backlit, shallow depth | **LE POT-DE-VIN LE REND CRÉDIBLE** |
| 20 | 2:05 | 7 s | Fountain pen signing a contract in close-up, warm lamplight, slow push-in | |
| 21 | 2:12 | 7 s | Steam train pulling out of a night platform, steam and gaslight, wide shot | *Direction Vienne* |
| 22 | 2:24 | 8 s | The Eiffel Tower again, identical framing to shot 1, slow push-in | **IL EST REVENU LA REVENDRE** |
| 23 | 2:38 | 9 s | Rope of knotted bedsheets hanging down a stone prison facade, daylight, wide shot | *27 jours de cavale* |
| 24 | 2:50 | 9 s | Close-up of a typewritten death certificate, the word "profession" visible, slow push-in, dust in light | **PROFESSION : APPRENTI VENDEUR** |

---

## AUDIO

**Voix off** — `generate_audio`, modèle `seed_audio`, voix masculine française, `speech_rate` légèrement sous la normale. Générer le script en **4 blocs séparés** (hook / acte 1-2 / acte 3 / acte 4-chute) plutôt qu'en un seul fichier : cela facilite le calage sur les plans et permet de refaire un bloc sans tout régénérer.

**Musique** — nappe instrumentale sobre, tension lente, à −18/−20 dB sous la voix. ⚠️ Le serveur Higgsfield **ne génère pas de musique pour usage général** (les modèles musicaux y sont réservés au pipeline de jeu). Il faut donc une source externe libre de droits.

**Mixage** — voix à −3 dB crête, musique −18 dB, aucun effet sonore ponctuel.

---

## MONTAGE

1. Assembler les 24 plans dans l'ordre, coupe franche, aucune transition.
2. Caler la voix off, ajuster les durées de plan au besoin (±1 s).
3. Incruster les sous-titres sur toute la durée — police unique, position constante.
4. Le plan 22 rejoue le cadrage du plan 1 : c'est le rappel de boucle.
5. Étalonnage final léger pour homogénéiser les 24 générations, qui ne sortiront pas parfaitement identiques.

---

## MÉTADONNÉES YOUTUBE

**Titre :** L'homme qui a vendu la Tour Eiffel. Deux fois.

**Description :**
> 1925 — Victor Lustig se fait passer pour un haut fonctionnaire du ministère des Postes et Télégraphes et « vend » la Tour Eiffel à la ferraille au marchand André Poisson. Humilié, celui-ci ne portera jamais plainte. Lustig reviendra tenter le coup une seconde fois.
>
> Les illustrations de cette vidéo sont générées par IA et purement artistiques : elles ne représentent pas les personnes réelles citées.
>
> Et toi, tu connaissais cette histoire ? Dis-moi en commentaire.

---

## ⚠️ VÉRIFICATION FACTUELLE AVANT PUBLICATION

Les faits ci-dessus (boîte roumaine, arnaque à Capone, double vente de la Tour, évasion, Alcatraz, mention « apprenti vendeur » sur le certificat de décès) sont documentés mais **je n'ai pas pu les vérifier dans une source primaire** : l'accès réseau de ma session est restreint. Contrôlez au moins les dates et les montants avant publication.

C'est la règle 6 appliquée en amont : le meilleur erratum est celui qu'on n'a pas à publier.
