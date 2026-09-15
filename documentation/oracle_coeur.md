> 💜 Le cœur : ce que l'Oracle lit, et avec quels mots.

Ce document est un **inventaire**, pas une spécification. Il rassemble en un
seul endroit les sous-catégories de valeurs, d'hameçons et de pondérateurs
éparpillées dans les versions successives, et regroupe sous chacune le
vocabulaire qui existe déjà.

Rien n'est inventé ici : chaque mot vient d'une source, notée en fin de bloc.

| marque | source |
|---|---|
| `2.5.1` | le lexique du moteur vivant, `src/oracle.js` |
| `V3` | `oracle_version/oracle_V3-avorton.md`, tables RED/ORANGE/GREEN |
| `V2` | `oracle_version/oracle_v2.md` |
| `feux` | la section FEU VERT / FEU ROUGE de ce document |
| `lexique` | LEXIQUE ÉMOTIONNEL DE DIANE, écrit à la main |
| `vécu` | relevé dans les réponses réelles des sauvegardes |

---

# La grille

```
Q1  première sensation      →  peur  ·  élan  ·  désintérêt
Q2  si ça se passe bien     →  récompense, par niveaux
Q3  si demain tu l'as pas   →  soulagement // regret, par niveaux
                               + ir/réversibilité  + répétition
Q0  la portée               →  des règles, pas des poids

par-dessus :  bonus / malus   →  valeurs  ·  hameçons
              et les pondérateurs, qui ne décident jamais seuls
```

---

# Q1 — première sensation

Trois compteurs indépendants. `élan` et `désintérêt` se soustraient ;
`peur` ne s'additionne pas, elle déclenche des règles.

## Élan

**Fort** — le corps et le cœur disent oui ensemble
> excit · hâte · j'ai hâte · trop hâte · j'adore · adore · kiffe · kiffer ·
> trop bien · super · génial · incroyable · fantastique · ça me fait vibrer ·
> j'en veux · tellement envie · grave envie · trop envie · enthousiasm ·
> euphor · joie · joyeu `2.5.1`
> motivé · énergie · élan · chaud · partant · vivant · dynamique `feux`
> ça me dit · envie grave · ça me ferait plaisir `lexique`

**Modéré** — l'ouverture sans l'enthousiasme
> why not · pourquoi pas · ça pourrait · ça peut · maybe · peut-être oui ·
> p'tet · bof mais · mouais mais · mmmh ok · curiosité · curieuse ·
> intéressée · intriguée · intéressant · sympa · pas dégueu ·
> ça me tenterait · tentée `2.5.1`
> tester · voir · découvrir · tenter · essayer `feux`

**Malgré l'obstacle** — l'élan qui passe en force
> dur mais allez allez il faut y aller `V3`

## Peur

> angoisse · angoissée · angoissan · angois · peur · peur de · j'ai peur ·
> panique · paniqu · paniquée · oppressée · oppresse · noeud au ventre ·
> boule au ventre · mal au ventre · stress · stressée · anxiété · anxieuse ·
> anxi · terreur · terrifée · effroi `2.5.1`
> flipper · inquiétude `feux`
> gorge serrée · souffle court · mal au cœur · corps tendu · corps lourd ·
> bloqué `lexique`

**La règle** — la peur seule freine, la peur avec de l'élan devient un signal
de valeur. C'est le `peur_excitation` du moteur, et la note ACT : *« peur +
envie = valeur, la peur est normale face au nouveau »*.

## Désintérêt

**Flemme** — trois états selon ce qui l'entoure
> flemme · flemme de · trop flemme · méga flemme · j'ai la flemme ·
> flemmasse · chiant · chiante · la chiantise · me soûle · me saoule ·
> ça m'emmerde · démotivée · pas envie du tout · bcp de flemme `2.5.1`

> | état | condition | source |
> |---|---|---|
> | inertie ignorable | flemme + un signal fort d'élan | `V3` |
> | vraie résistance | flemme + « peur de m'ennuyer », « ça me soûle » | `V3` |
> | flemme neutre | flemme seule | `V3` |

**Tiédeur**
> bof · mouais · meh · moyen · beurk · pas folle · pas dingue · mmh ·
> mmmmh · hm · hmm · pas convaincue · sceptique · pas terrible ·
> pas ouf `2.5.1`
> pff · pfffff `lexique`

**Refus net**
> pas envie · pas vraiment envie · pas trop envie · zéro envie `2.5.1`

---

# Q2 — si ça se passe bien : la récompense

C'est ici que les **valeurs** se lisent. Le niveau dit l'intensité, la valeur
dit la nature.

**Récompense pleine**
> mega fière · méga fière · trop fière · super fière · fière · fierté ·
> s'amuse de fou · on s'amuse · kiffe grave · kiffe trop · kiffe à fond ·
> adore · à fond · complètement dedans · dans mon élément · trop bien ·
> super bien · génial · incroyable · fantastique · heureuse · épanouie ·
> vivante · énergisée · accomplie · réalisée · satisfaite `2.5.1`

**Récompense creuse** — l'option qui remplit le temps sans rien rapporter
> passer le temps · tuer le temps · en attendant · pour m'occuper ·
> histoire de · faute de mieux · rien d'autre à faire · par défaut `2.5.1`

---

# Q3 — si demain tu l'as pas fait

Trois lectures superposées sur la même réponse.

## Regret

**Fort**
> honteu · honte · honteuse · dégoûtée · dégoutée · dégoût · fâchée ·
> en colère contre moi · nulle · nulle de chez nulle · trop nulle ·
> trop deg · méga deg · triste · tristesse · chagrin · frustrée ·
> frustration · déçue de moi · déçue · pas fière · pas contente de moi ·
> regret · je regretterais · j'aurais regretté · j'aurais raté ·
> j'aurais manqué `2.5.1`

**Modéré**
> dommage · un peu dommage · c'est dommage · maybe deg · un peu deg ·
> légèrement deg · un peu triste · légèrement déçue · pas idéal ·
> pas top · j'aurais aimé · j'aimerais quand même `2.5.1`

**Nul** — l'indifférence, qui est une réponse
> je m'en fous · osef · m'en fiche · m'en bat · rien · rien du tout ·
> que dalle · change rien · rien de spécial · pareil · même chose ·
> peu importe · bah rien · pff rien `2.5.1`

## Soulagement

**Fort** — ne pas le faire ferait du bien : c'est un signal, pas de la fatigue
> soulagée · soulagement · soulage · ouf · tranquille · en paix · relax ·
> zen · repos · reposée · relaxée · libérée · mieux · mieux comme ça ·
> mieux sans · contente · heureuse · bien `2.5.1`
> apaisé · calme · posé · ça passe · c'est fait · au moins c'est clair ·
> j'ai dit ce que j'avais à dire · j'ai essayé · j'assume · j'avance `lexique`

**Léger** — ne pas pénaliser, c'est du bruit
> un poil coupable · un peu coupable `2.5.1` `V3`

## Irréversibilité

L'axe le plus discriminant du corpus : *« Q3 = je peux toujours le faire
≈ option déprioritisable »*, relevé 5-6 fois.

**Réversible — je peux toujours**
> je peux toujours · au pire · pas grave · on verra · réversible `feux`
> au pire c'est pas grave · pas la fin du monde `2.5.1`

**Irréversible — l'occasion ratée**
> rare · unique · jamais plus · chance unique · maintenant ou jamais ·
> opportunit · occasion `2.5.1`
> pas sûre s'il y a d'autres occasions `V3`
> rarement · longtemps qu'on se rate `V3`

## Répétition

Contredit un « ça ne comptera pas » : si ça revient, ça compte.

> encore · toujours · à chaque fois · souvent `feux`
> procrastin · ça traîne · encore traîner · traîne depuis `2.5.1`
> depuis longtemps · en attente `V3`
> rebelote `vécu`

---

# Les valeurs

Ce vers quoi je VEUX aller, même si c'est difficile ou effrayant `ACT`.
Bonus à plat — la valeur qualifie, elle ne pèse pas plus lourd d'elle-même.

| Sous-catégorie | Vocabulaire | Source |
|---|---|---|
| **Créativité / expression** | créatif · créer · créativité · création · dessiner · peindre · imagin · moment créatif · artistique | `2.5.1` `V3` |
| **Apprentissage / croissance** | appren · apprendre · appris · découv · découvert · progressé · évolué · compris · progresser · développement · débloquer · consolider | `2.5.1` `V3` |
| **Connexion / intimité** | connexion · lien · rapprochement · complicité · ensemble · se rapprocher · rigoler ensemble · moment · potes · relationnel · amitié | `2.5.1` `V3` |
| **Liberté / authenticité** | libre · liberté · autonome · indépendante · moi-même · vraiment moi · authentique · autonomie | `2.5.1` `V3` |
| **Fierté / estime** | fière · fierté · mega fière · respect · digne · assumé · ok avec moi-même · accomplie · réalisée | `2.5.1` `feux` |
| **Plaisir** | kiff · plaisir · envie · fun · agréable · cool · bien · joyeux · léger · s'amuse de fou · kiffe | `feux` `2.5.1` |
| **Curiosité** | curieux · curiosité · tester · voir · découvrir · tenter · essayer · intriguée | `feux` `2.5.1` |
| **Repos réel** | me reposer vraiment · reprendre des forces · vrai repos · respirer · pause | `V3` |
| **Aventure / nouveauté** | s'amuser · aventure · stimulant · actif · actrice · vivante · énergisée | `V3` `2.5.1` |
| **Clarté** | clair · simple · évident · logique · fluide · naturel | `feux` |
| **Projet / consolidation** | projet · consolider · situation · remotiver · avancer · debloquer | `V3` `2.5.1` |

> `Clarté` et `Repos réel` sont nommées mais n'ont encore jamais été lues par
> un moteur. `Aventure` non plus, sauf par ricochet.

---

# Les hameçons

Ce qui m'accroche malgré moi : peur, culpabilité, validation externe `ACT`.
Malus.

| Sous-catégorie | Vocabulaire | Source |
|---|---|---|
| **Obligation déguisée** | je devrais · il faut que · il faut · obligation · obligée · je dois · on attend de moi · c'est mon rôle · sinon · si je fais pas · j'ai dit que · j'ai promis · j'avais dit · c'est la chose logique · logique de · normal de · me trahir | `2.5.1` `V3` |
| **Injonctions sociales** | tout le monde · tout le monde y va · sois raisonnable · anormal · bizarre de | `2.5.1` + prose ci-dessous |
| **Culpabilité** | coupable · culpabilité · culpab · honte · honteuse · mauvaise conscience · remords · j'aurais dû · aurais dû faire · je m'en veux | `2.5.1` `lexique` |
| **Pression sociale / regard** | gênée · gêne · mal à l'aise · awkward · bizarre · chelou · ils vont · ils vont penser · vont penser · je les reverrai · je les verrai · on se voit · jugement · jugée · mal vue · décevoir · vexer · blesser | `2.5.1` |
| **Procrastination** | procrastin · ça traîne · encore traîner · traîne depuis · depuis longtemps · en attente | `2.5.1` `V3` |
| **Dépendance à un tiers** | elle va · mon conseiller · mon boss · attendre qu'ils répondent | `V3` `vécu` |
| **Auto-jugement** | ridicule · faible · bête · naïve · pathétique · pas malin · pas digne · pas fière · j'abuse · j'exagère · je me respecte pas | `lexique` |
| **Rationalisation** | maybe si… · ça pourrait… · peut-être oui si… · risque que… · au quotidien | `lexique` |
| **Ambivalence** | oui mais non · both / neither · ça dépend · d'un côté… de l'autre… | `lexique` |
| **Peur de l'inaction** | peur de couler · inactive · rien faire · peur d'être inactive | `V3` |
| **Manque / dépendance** | besoin · manque · vide · dépendance · accro · attaché | `feux` |
| **Malaise** | mal à l'aise · gênant · chelou · bizarre · froid · lourd · oppressant · étouffant | `feux` `lexique` |

## Ceux que tu as nommés en prose, sans vocabulaire encore

Écrits de ta main dans ce document, jamais traduits en mots-clés :

- **La peur de déranger** les autres, et donc de ne pas demander.
- **La persévération** : rester fixé sur un plan même quand il n'est plus
  pertinent.
- **Ne pas écouter mes besoins**, ou le corps (douleurs).
- **« Sois raisonnable »** = risque et gros trigger.
- **« Anormal » = alarm bell** — quand Diane dit qu'une chose lui semble
  « anormale » ou « bizarre » à faire, c'est souvent la tête ou le regard des
  autres qui parle, pas elle.
- **Risque de rationalisation a posteriori.**

---

# Les pondérateurs

Ils modifient le poids, ils ne décident jamais seuls.

## Multiplicateurs

| | Vocabulaire | Source |
|---|---|---|
| **Intensité** | très · trop · à fond · énormément · grave · méga · mega · carrément | `feux` `2.5.1` |
| **Répétition** | encore · toujours · à chaque fois · souvent · rebelote | `feux` `vécu` |
| **Projection** | j'imagine · je me vois · si jamais · et après | `feux` |

## Diviseurs

| | Vocabulaire | Source |
|---|---|---|
| **Réversibilité** | au pire · pas grave · on verra · réversible · je peux toujours | `feux` `2.5.1` |
| **Relativisation** | au pire c'est pas grave · pas la fin du monde · osef · je m'en fous · bah · c'est juste · c'est rien · c'est pas grave · j'aurais oublié · ça compte pas vraiment | `2.5.1` |
| **Distance** | un peu · moyen · bof · pas tant que ça | `feux` |

## Neutraliseurs

| | Vocabulaire | Source |
|---|---|---|
| **Confusion** | je sais pas · flou · confus · perdu · j'en sais rien | `feux` `2.5.1` |
| **État limite** | à bout · trop mal · au fond du trou | `feux` |
| **Exclusions** | un poil · un peu — annulent certains motifs au lieu de les pondérer | `V3` `2.5.1` |

---

# Sources externes

## ACT (Acceptance and Commitment Therapy)
- **Valeurs** : ce vers quoi je VEUX aller (même si c'est difficile/effrayant)
- **Hameçons** : ce qui m'accroche malgré moi (peur, culpabilité, validation externe)
- **Nuance clé** : « peur + envie » = valeur (la peur est normale face au nouveau)

## « Decisive », frères Heath
Leur premier péché de la décision est le *narrow framing* : poser le problème
en « est-ce que je fais X, oui ou non ». Le tableau est structurellement
binaire — et le commentaire du 13/01 (« là on arrive à un moment où il
faudrait proposer d'ajouter une option C 🙂 ») redécouvre exactement ça.

## Théorie du regret (Bell, Loomes & Sugden ; version populaire chez Bezos)
Le regret anticipé est un meilleur guide que la préférence du moment. C'est ce
qui justifie que Q3 soit l'échelle la plus lourde — la leçon du 1er mai le
disait déjà, et plus clairement.

## Affective forecasting (Gilbert & Wilson)
On prédit mal ce qu'on ressentira. C'est l'argument pour que Q0 puisse
*écraser* Q1 : la sensation présente est une donnée peu fiable dès que
l'échéance s'allonge. Le Q0 à dix jours ressemble à la règle « 10/10/10 » de
Suzy Welch.

## Théorie des cuillères
Le coût et la récupération se comptent en PV. Le trésor, lui, n'est pas de
l'énergie.

## Robyn Dawes, « The robust beauty of improper linear models » (1979)
Les modèles linéaires à très peu de variables, avec des poids grossiers,
battent régulièrement le jugement expert *et* les modèles finement optimisés.
Parce que les poids finement optimisés sont ajustés au passé, et que le futur
n'est pas le passé. **Les modèles de décision qui survivent sont petits.**

---

# Ce que les sauvegardes ont appris

| Signal | Exemple |
|---|---|
| **La rareté doit peser lourd** | « le truc qui gagne beaucoup et qui est rare » ; le 1er mai « ça n'a lieu qu'une fois par an » |
| **Le regret bat la flemme** | « mieux vaut essayer de faire quelque chose qui me donne bof envie que de regretter de pas l'avoir fait » |
| **Q3 = « je peux toujours le faire » ≈ option déprioritisable** | revient 5-6 fois, très discriminant |
| **« Aucun des deux » est parfois faux** | le week-end à Lyon : il n'y avait pas de 3ᵉ possibilité, le bot ne le sait pas |
| **… mais parfois c'est exactement le bon move** | « là on arrive à un moment où il faudrait proposer d'ajouter une option C 🙂 » |
| **Le calcul est mal pondéré** | Lyon : beaucoup de négatif d'un côté, neutre de l'autre → le verdict n'a « pas de sens » |
| **Certaines décisions sont trop grosses pour un verdict** | Inde/Asturias : mots « projet, temps, réfléchir » + émotions fortes → l'oracle devrait **nommer le dilemme**, pas juste trancher |
| **Nommer la peur sous-jacente** | « peut-être nommer ma peur d'être inactive » |
| **Les obligations écrasent l'envie** | le RDV conseillère : « bien sûr qu'il faut honorer un rendez-vous même si on n'a pas envie » |
| **Aveu d'incertitude assumé** | « l'oracle n'a pas assez d'éléments pour trancher » → « Pile ou face » |
| **Q1 = peur = important** | « ça me fait peur » accompagne presque tous les choix notés _good_ (l'admin, le lac, Asturias) |

**Corps fatigué ≠ pas envie.** Parfois on est crevé mais on VEUT quand même
faire un truc. Si « demain sans » = regret fort, l'envie dépasse la fatigue.

---

# La faille connue de Q0

Faire une sortie avec mes amies, je ne dirais pas forcément « dans 10 jours ça
compte » — pourtant ça peut créer un souvenir pour toujours. Pareil pour mon
hygiène : dans 10 jours ça ne compte pas forcément, et en même temps c'est
important.

---

# Ailleurs

- La **liste brute de vocabulaire** (861 entrées, non triées) est restée dans
  `oracle_cerveau.md`, sous `# vocabulaire`. Rien n'en a été supprimé.
- Les **phrases** de l'Oracle sont dans `oracle_phrases.md`.
- Les **lexiques complets** version par version sont dans
  `oracle_version/`.
