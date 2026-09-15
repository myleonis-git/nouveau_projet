> 🧠 La logique : ce que l'Oracle calcule, et avec quels poids.

# Récapitulatif de la logique

## Les quatre questions

| | Question | Ce qu'on en lit | Nature |
|---|---|---|---|
| **Q1** | Première sensation ? | **peur** · **élan** · **désintérêt**, trois compteurs séparés | élan et désintérêt s'additionnent ; la peur déclenche des règles |
| **Q2** | Si ça se passe bien ? | **récompense**, par niveaux, et la **valeur** qu'elle sert | points + étiquette |
| **Q3** | Si demain tu l'as pas fait ? | **soulagement // regret** par niveaux, **ir/réversibilité**, **répétition** | trois lectures sur la même phrase |
| **Q0** | Dans 10 jours, ça compte ? | **la portée** — oui / peut-être / non | des règles, pas des points |

## Les trois monnaies

| | Unité | Entre dans le score ? |
|---|---|---|
| **Coût** | PV dépensés | oui, s'il dépasse l'énergie disponible |
| **Récupération** | PV rendus | non — comptée à part depuis la 2.5.1 |
| **Trésor** | ni PV ni points | départage seulement |

## Les verdicts

| Verdict | Quand |
|---|---|
| **Une voie** | un écart net entre les scores |
| **La pièce** | ça ne comptera pas : pile ou face assumé |
| **Les cartes** | ça compte, mais rien ne départage |
| **Aucune des deux** | toutes les voies sous zéro |

---

# Combien faire peser quoi

## Ce que dit la recherche

**1. Des poids grossiers battent des poids ajustés.**
Dawes montre que des modèles linéaires à poids égaux, ou même arbitraires,
battent régulièrement le jugement expert *et* les modèles finement optimisés.
Ce qui compte, c'est de savoir **quelles variables regarder et dans quel
sens** — pas de trouver le bon coefficient. Les poids finement ajustés le sont
au passé, et le futur n'est pas le passé.

→ **Des entiers simples. Jamais un poids réglé sur les 27 dilemmes passés.**

**2. Le regret doit peser plus lourd que l'envie.** Trois sources convergent :

- L'aversion à la perte : λ ≈ 2,25 chez Tversky & Kahneman (1992) — une perte
  pèse deux fois une équivalent gain. Le chiffre est discuté, des
  méta-analyses trouvent parfois bien moins, mais le sens ne bouge pas.
- *Bad is stronger than good* (Baumeister et al., 2001) : le négatif l'emporte
  dans presque tous les domaines mesurés, avec un rapport de 2 à 5 selon le
  contexte.
- Surtout : le **regret anticipé** prédit le comportement **mieux que les
  autres émotions négatives** (Brewer et al., 2016 — méta-analyse, 81 études,
  45 618 personnes ; r = .50 avec l'intention, .29 avec le comportement). Et
  le **regret d'inaction** — littéralement la Q3 — a une association plus
  forte qu'on ne le croyait.

→ **Regret fort ≈ 2 × élan fort.**

> ⚠️ Le moteur actuel fait l'inverse : élan fort = **+5**, regret fort =
> **+4**. Les sauvegardes disaient déjà le contraire (« mieux vaut essayer
> quelque chose qui me donne bof envie que de regretter de pas l'avoir
> fait »).

**3. La peur ne doit pas être un simple malus.**
L'évitement expérientiel — fuir ce qu'on redoute — est associé à l'anxiété et
à la dépression avec des effets moyens à forts (r = .34 à .56 ; méta-analyse
de 441 études, 135 347 participants). Retirer des points dès qu'une peur
apparaît, c'est pousser mécaniquement vers l'évitement, exactement le schéma
que l'ACT identifie comme coûteux.

→ **La peur ne s'additionne pas. Elle déclenche des règles.** C'est déjà la
décision prise, et elle est fondée.

**4. Trois à cinq niveaux par échelle, pas plus.**
En dessous de 5 points on perd de l'information, au-dessus de 7 le gain
devient marginal (Preston & Colman). Pour une échelle remplie en texte libre,
3 ou 4 niveaux par axe suffisent largement.

## Poids proposés

Grossiers, entiers, dans l'esprit de Dawes. À discuter, pas à appliquer.

| Signal | Lu en | Poids | Pourquoi |
|---|---|---|---|
| Regret fort | Q3 | **+6** | le meilleur prédicteur de la littérature *et* du corpus |
| Regret modéré | Q3 | **+2** | |
| Regret nul | Q3 | **−2** | l'indifférence est une réponse |
| Soulagement fort | Q3 | **−5** | ne pas le faire soulagerait : signal, pas fatigue |
| Élan fort | Q1 | **+3** | moitié du regret fort, conforme à λ ≈ 2 |
| Élan modéré | Q1 | **+1** | |
| Désintérêt | Q1 | **−1** à **−2** | selon l'état de la flemme |
| Refus net | Q1 | **−3** | |
| Récompense pleine | Q2 | **+3** | |
| Récompense creuse | Q2 | **−1** | |
| Valeur servie | Q2 | **+1** à plat | elle qualifie, elle ne pèse pas plus |
| Hameçon | Q1 / Q3 | **−2** chacun | |
| Peur | Q1 | **0** | règles seulement |

## Et Q0 ?

Q0 est **globale** : une seule réponse pour toute la quête. Un multiplicateur
appliqué à toutes les voies ne change donc pas leur ordre.

```
A = 6, B = 2   →  ×2  →  A = 12, B = 4     A gagne toujours
```

Mais il change les **écarts**, donc la catégorie du verdict :

```
A = 6, B = 2   écart 4  →  « c'est serré »
        ×2     écart 8  →  « c'est net »
```

→ Un multiplicateur Q0 ne peut pas désigner une autre voie, mais il peut
changer la confiance de l'Oracle, et faire basculer « aucune des deux ». La
relativisation (÷2 sur « au pire c'est pas grave ») fait déjà exactement ça.

| réponse | portée | effet proposé |
|---|---|---|
| Oui | `high` | ×1,5 sur les écarts — l'Oracle tranche plus volontiers |
| Peut-être | `medium` | ×1 |
| Non | `low` | verrou : pile ou face, sans analyse de rang |

## La seule validation honnête

Ces poids ne peuvent pas être prouvés sur les 27 dilemmes passés : les y
ajuster, c'est précisément ce que Dawes déconseille, et l'expérience de
surapprentissage l'a montré — une avance de 23 points s'est évaporée sur
8 dilemmes inédits. **Un poids se défend, il ne se règle pas.** La mesure
viendra des dilemmes à venir, pas de ceux qui ont servi à le construire.

---

# Décisions encore ouvertes

- **Amitié** : valeur à part entière, ou nuance de la connexion ?
- **Q0** : multiplicateur sur les écarts, ou règles seules ?
- **Répétition** : contredit-elle « ça ne comptera pas » ? (décidé oui, à câbler)
- **Irréversibilité** : un cran de Q3, pas un pondérateur (décidé, à câbler)

---

# Interprétation

#### q1
#### q2
#### q3
#### q0
'non' catégorique = pile ou face

# recommendation
Voie A,B,C,D
Aucun des deux X
Pile ou face Y
%%Réfinir les différentes catégories de l'Oracle:
clear / weak / energy (mais en vrai j'utilise peu cette fonctionnalité)%%
Créer un code par recommendation, pour permettre à l'App d'extraire ensuite une phrase random dans un second fichier oracle_words

# feedback
#### Followed Oracle
null pour pile ou face
true si recommandation ni l'un ni l'autre = decision aucun des deux / autre
#### OracleWasRight:
true si
- recommandation = choix & satisfaction Oui (3/3)
- recommandation =/= choix & satisfaction Non ou Bof (1/3 ou 2/3)

# vocabulaire
mmh
abandon
abattu
abraser
absurde
abus
abîmé
accord
accro
achat
actif
action
adhérer
adhésion
admiration
admirer
adore
adrenaline
affect
agacé
agir
agressif
aide
aimer
aisance
alarme
alerte
alignement
aligné
allegresse
allumer
aléatoire
ambigu
ambiguïté
ambivalence
ambivalent
amour
amusant
amusement
améliorer
angoisse
animé
annuler
anticiper
anxiété
apaisant
apathie
apathique
appartenance
appartenir
apprendre
approche
apprécier
arbitrage
arbitraire
arbitrer
ardeur
argent
arrêt
arrêter
art
assumer
assuré
attente
attention
attirer
au pire
aujourd'hui
authenticité
authentique
autonomie
autre
aventure
avide
avoir
avouer
bafoué
bah
bien
bien-être
blessé
bof
bon
bonheur
bouger
boulot
bourreau
bousculé
boussole
brave
brillant
briser
béatitude
calme
calmer
capable
casser
catastrophe
chaleur
chance
change
changer
chaos
chaud
chelou
choix
choquant
circonstances
clair
clarté
coeur
cohérence
cohérent
coincé
colère
combattre
comfort
commencer
commun
complicité
compliqué
comprendre
compétence
concentré
confiance
confiant
confort
connaissance
connecter
conscience
conseil
consentement
consolider
construire
content
continu
contrôle
convaincre
copain
corps
correct
coupable
courage
courant
courir
cri
critique
crucial
créatif
création
créer
culpabilité
curieu
curieux
curiosité
dangereux
deg
demain
destruction
deuil
devoir
difficile
digne
dimension
dire
discipline
discordance
discordant
discret
disponible
dissiper
divertir
dois
dommage
doute
doux
droit
drole
dysphorie
débloquer
décider
décision
défaut
défendre
défi
dégout
déjà
délire
démarrer
démotivé
déménager
dépasser
dépendance
dépendant
dépourvue
déprimé
déranger
désaccord
désastre
désespoir
désir
désolant
désolé
désordre
déséquilibre
détacher
détendre
détruire
déçu
engagé
ennuyeux
enrichir
enseigner
entendre
enthousiasme
enthousiaste
entier
entouré
envie
environnement
erreur
espoir
essayer
essentiel
estime
euphorie
exact
excit
excité
exclusif
excuse
exiger
exister
explorer
exposer
exprimer
expérience
extraordinaire
fachee
facile
faire
faire confiance
faire face
faire peur
faire plaisir
faire semblant
faire un choix
faire un effort
faire un geste
faire un pas
faire un tour
faire un travail
faire un voyage
fatigué
faute
faux
fier
fierté
fière
fiévreux
flemme
flou
fluide
folie
force
forcer
fort
fou
fous
fragile
franchement
frileux
frilosité
froid
frustration
fréquent
fuite
fun
furieux
futur
fébrilité
gagner
gentil
gestion
grand
grand chose
gratitude
gratuit
grave
gravité
gronder
groupe
grâce
guérir
gâcher
génial
généreux
gênant
gêné
haine
harmonie
harmonieux
haut
heureux
hier
honneteté
honte
horrible
humeur
humour
hypocrisie
hypocrite
hâte
hésiter
idéal
idée
il faut
illusion
image
imaginer
imitation
immobile
immédiat
impact
impatient
impatienter
importan
impossible
impression
improviser
impulsion
inattendu
incertain
incertitude
incohérent
incongruence
incroyable
indifférent
indispensable
individuel
indécis
influence
influencer
injuste
injustice
innovation
inquiétude
insatisfait
inspiration
instable
instant
instinct
insuffisant
intelligence
intense
intention
interdit
interrompre
intervention
intimité
intuition
intérêt
inutile
investir
irrité
isoler
joli
jouer
joyeux
juger
juste
justice
kiffe
kiffer
laisse tomber
laissez-faire
langage
lassé
libre
libérer
limite
logique
loin
loisir
long
lourd
lourdeur
loyal
lucide
lumière
lutter
luxueux
lâcher
lâcher prise
lâcheté
léger
légereté
magique
magnifique
mal
malade
malheur
malin
manipuler
manque
marche
marre
maîtriser
meilleur
membre
menace
mener
mentir
mesure
mettre
mieux
milieu
minimal
minimiser
momentum
monde
monotone
montrer
morale
morceau
motivation
mouvement
moyen
multitâche
méditer
mélancolie
mépriser
mériter
naturel
nerveux
net
neuf
neutraliser
neutralité
nominalisé
nouveau
nouveauté
noyer
nuage
nul
nécessaire
nécessité
négatif
négocier
obligation
obligé
obscur
obscurité
obsession
obstacle
obtenir
occasion
occupé
opinion
opportunité
optimiste
ordre
organiser
orgueil
original
osef
oser
oubli
oubliant
oublier
oublié
oubliée
oubliées
oubliés
ouvrir
paisible
panique
parfait
parler
partager
partir
passion
passionné
passé
patience
patient
patienter
pause
peine
penser
perdre
perfection
perte
perturbé
pesanteur
peser
peur
peut-etre
peuvent
pff
phobie
physique
piquer
pire
piège
plaisir
plan
plein
pleurer
plus
pouvoir
prendre
pressentiment
presser
pression
problème
procrastination
procrastiner
produire
profiter
profond
profondeur
progrès
projet
promesse
promettre
propre
protéger
précaire
précarité
précaution
précieux
précis
préciser
précision
précédent
prédire
préférence
préférer
préparer
présent
prétendre
prétendu
prétendue
prétendus
prétentieuse
prétentieuses
prétentieux
prétention
prêt
prêt à
putain
quand
quantité
quartier
question
questionner
quitter
quiétude
quotidien
raison
raisonnable
raler
rapide
rapidité
rare
rareté
rassurant
rassurer
rassuré
recharge
recharger
reconnecter
reconnecté
recul
reculer
refuser
regard
regarder
regret
regretter
rejet
rejeté
remobiliser
remotiver
richesse
ridicule
rien
rigide
rigidité
rigolo
rigueur
risque
risquer
rituel
robuste
robustesse
rompre
râler
réaction
réagir
réaliser
réaliste
réalité
récompense
réconfort
réconforter
réfléchir
résonance
résonner
réussir
réussite
réveil
réveiller
révolter
révolté
révolution
révolutionner
rêve
rêver
saboter
sacré
sadique
sagesse
saisir
santé
satisfaction
satisfait
sauver
serein
seul
seule
seulement
silence
simple
simplicité
sincère
sincérité
situation
société
soi
soin
solide
solidité
solitude
solution
sommeil
sororité
souci
souhait
souhaiter
soulager
souple
souplesse
sourire
souvenir
souvent
spontané
spontanéité
stabilité
stimuler
stress
stressant
stressante
stressants
stressé
stressée
stressées
stressés
stupide
stupéfaction
stupéfait
stupéfiante
stupéfier
succès
suffire
suffisance
suffisant
suffit
suffoquer
suivre
super
superficiel
supprimer
surface
surmonter
surprenant
surprendre
surpris
surprise
survivre
suspicieuse
suspicieuses
suspicieux
suspicion
système
systématiquement
systémique
sécurité
sérieusement
sérénité
tactique
talent
tangible
tanker
tant pis
tard
tension
tenter
terrible
tester
timide
timidité
timing
tirer
tirer parti
tirer profit
tirer vers le bas
tirer vers le haut
tolérance
tolérer
tomber
tordre
tort
toucher
toujours
tourment
tourmenter
tout
tout de suite
tout faire
tout le monde
tout le temps
tout seul
tout simplement
tout à coup
tout à fait
tout à l’heure
toxique
tracas
tracasser
tragique
trahison
trancher
tranquille
tranquilliser
tranquillité
transcender
transformation
transformer
transgresser
transgression
transparence
transparent
travail
travailler
trembler
triste
tristesse
tromper
trop
trou
trouillard
trouver
très
tuer
turbulence
turbulent
tâche
un poil
urgence
urgent
utile
utiliser
utilité
vague
vain
vaincre
valable
valeur
valider
valoir
valoir le coup
valoir mieux
vanité
variété
vaste
vertige
vibrer
victoire
vidée
vie
vieillir
vif
vigilance
vigilant
vigoureux
vigueur
village
vindicatif
violence
violent
virer
virtuose
visible
vision
visuel
vital
vitalité
vite
vitesse
vivace
vivacité
vivant
vivement
vivifier
vivre
vocation
voeu
voeux
vouloir
voyage
voyager
vrai
vulnérabilité
vulnérable
vécue
véhémence
véhément
véhémentement
véhémenter
vérifiable
vérifier
véritable
véritablement
vérité
why not
zeste
zone
zoomer
zénitude
zéro
à fond
échec
éclaircir
éclater
écoeuré
économie
écouter
énergie
énervé
éprouver
équilibre
équipe
étonnant
étonné
étourdi
étourdissement
étranger
évidence
éviter