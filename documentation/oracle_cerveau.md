> 🧠





# detection vocabulaire
Attention envie =/= pas envie

# interprétation 

#### q1
#### q2
#### q2
#### q0:
'non' catégorique = pile ou face



## Les quatre questions

**Q1 — trois compteurs séparés**, deux niveaux chacun (petit 2 / fort 4) :

```
ÉLAN      ce qui tire vers l'avant
PEUR      l'alarme du corps
INERTIE   ce qui repousse, sans peur

envie = ÉLAN − INERTIE   → entre dans l'addition
peur                     → n'entre PAS dans l'addition, sert aux règles
```

Justifié par tes données : **15 % de tes réponses mêlent élan et peur.** Un seul axe les annulerait.

**Q2** — une seule échelle, positive, minimum 0. Pas de cohabitation observée, un compteur suffit.

**Q3** —
INTENSITÉ      soulagement · osef · un peu frustrée · regret net
IRRÉVERSIBILITÉ   je peux toujours  ←→  occasion ratée
REPETITION

**Q0 (la portée)** — **ne donne aucun point**. C'est arithmétique : elle est globale, donc des points fixes s'annulent entre les options. Elle agit en **règles** (plutôt qu'en poids, à mon avis révisé).

## Les facteurs

- **Énergie** : coût net = coût − gain. Si déficit **et** pas de vert fort → pénalité. Si vert fort → on note le dépassement mais **on ne pénalise pas** (la règle du lac). C'est ta V2.5, je n'ai rien de mieux.
- **Coût comparé** → départage
- **Gain** → **départage uniquement**, jamais prioritaire sur tes mots

## Bonus / malus — ±1 plat, jamais ajustés individuellement

- **valeurs** (ta liste validée en amont) : +1 par mot, plafonné, et **taggées pour le journal**
- **hameçons** : −1
- **engagement** : détecté aux **verbes relationnels** (« j'ai dit », « m'attend », « compte sur moi ») → +1
- **culpabilité** : détectée aux **impersonnels** (« il faut que », « normal de », « tout le monde ») → −1
- **Les deux peuvent se déclencher ensemble** — net zéro, et la phrase pose la question. Le cas ambigu devient une information, pas un bug.

## Verdict

- égalité → **pas plus de granularité** (ça ne réglerait rien : parfois tes deux réponses sont identiques), mais **départage par le gain**
- **pièce** = « ça ne comptera pas, arrête de calculer »
- **cartes** = « ça compte, et je n'ai pas assez d'éléments » — plus solennel

## Deux principes

> **Une règle se teste. Un poids se défend.**  
> Donc : beaucoup de règles, peu de poids.

> **Suite de régression rejouée à chaque changement.**  
> C'est ce qui aurait attrapé les trois régressions de la V2.5.

---

**deux règles qui contredisent Q0** :

|||
|---|---|
|**répétition**|« ça ne comptera pas » est faux pour les choses qui reviennent|
|**peur + regret**|la peur ne disqualifie pas quand ça compte|


# Combien faire peser quoi

Recherche faite le 15/09, à confronter à l'échelle ci-dessus.

## Quatre résultats

**1. Des poids grossiers battent des poids ajustés.**
Dawes montre que des modèles linéaires à poids égaux, ou même arbitraires,
battent régulièrement le jugement expert *et* les modèles finement optimisés.
Ce qui compte, c'est de savoir **quelles variables regarder et dans quel
sens**, pas de trouver le bon coefficient — parce qu'un coefficient fin est
ajusté au passé, et que le futur n'est pas le passé.

→ Ton « ±1 plat, jamais ajusté individuellement » est exactement ça.
Et ton « un poids se défend » aussi.

**2. Le regret doit peser environ deux fois l'élan.** Trois sources
convergent :

- L'aversion à la perte : λ ≈ 2,25 chez Tversky & Kahneman (1992). Le chiffre
  est discuté — des méta-analyses trouvent parfois bien moins — mais le sens
  ne bouge pas.
- *Bad is stronger than good* (Baumeister et al., 2001) : le négatif l'emporte
  dans presque tous les domaines mesurés, rapport de 2 à 5.
- Surtout : le **regret anticipé** prédit le comportement **mieux que les
  autres émotions négatives** (Brewer et al., 2016 — méta-analyse, 81 études,
  45 618 personnes ; r = .50 avec l'intention, .29 avec le comportement). Et
  le **regret d'inaction**, littéralement ta Q3, a une association plus forte
  qu'on ne le croyait.

→ Si Q1 fort vaut **4**, Q3 regret net devrait valoir **8**, pas 4.
C'est le seul endroit où la recherche demande de casser la symétrie des
échelles. Ta propre leçon disait déjà la même chose : *« mieux vaut essayer
quelque chose qui me donne bof envie que de regretter de pas l'avoir fait »*.

**3. La peur ne doit pas être un simple malus.**
L'évitement expérientiel — fuir ce qu'on redoute — est associé à l'anxiété et
à la dépression avec des effets moyens à forts (r = .34 à .56 ; méta-analyse
de 441 études, 135 347 participants). Retirer des points dès qu'une peur
apparaît, c'est pousser mécaniquement vers l'évitement, exactement le schéma
que l'ACT identifie comme coûteux.

→ Ta décision — la peur n'entre pas dans l'addition, elle sert aux règles —
est fondée, pas seulement intuitive.

**4. Deux niveaux par compteur, c'est peu mais défendable.**
En dessous de 5 points d'échelle on perd de l'information, au-dessus de 7 le
gain devient marginal (Preston & Colman). Ton petit 2 / fort 4 donne, une
fois `élan − inertie` calculé, une échelle à 5 positions (−4 −2 0 +2 +4).
C'est le plancher de la zone utile, pas en dessous.

## Sources

- Dawes, *The robust beauty of improper linear models in decision making* (1979)
- Tversky & Kahneman, *Advances in prospect theory* (1992) — λ ≈ 2,25
- Baumeister, Bratslavsky, Finkenauer & Vohs, *Bad is stronger than good* (2001)
- Brewer, DeFrank & Gilkey, *Anticipated regret and health behavior* (2016)
- Preston & Colman, sur le nombre de points d'échelle (2000)
- Méta-analyse sur l'évitement expérientiel (441 études, 2022)

## La seule validation honnête

Ces poids ne peuvent pas être prouvés sur les dilemmes déjà enregistrés : les
y ajuster est précisément ce que Dawes déconseille, et l'expérience 3 du labo
l'a montré — une avance de 23 points s'est évaporée sur 8 dilemmes inédits.
La mesure viendra des dilemmes à venir, pas de ceux qui ont servi à
construire le barème.

---

# recommendation
Voie A,B,C,D
Aucun des deux X
Pile ou face Y
%%Réfinir les différentes catégories de l'Oracle:
clear / weak / energy (mais en vrai j'utilise peu cette fonctionnalité)%%
Créer un code par recommendation, pour permettre à l'App d'extraire ensuite une phrase random dans un second fichier oracle_words

# dénouement
#### Followed Oracle
null pour pile ou face
true si recommandation ni l'un ni l'autre = decision rien  / autre

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