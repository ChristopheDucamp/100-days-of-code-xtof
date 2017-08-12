Le journal de mes "100 Days Of Code" (pour le distinguer du [repo principal](https://github.com/ChristopheDucamp/100-days-of-code) et permettre aux personnes de forker une version propre)

# #100DaysOfCode Log - Round 1 - [xtof](http://xtof.me)

Le journal de mon défi #100DaysOfCode. Démarré le lundi 24 juillet 2017.

## Log

![GitHub-ChristopheDucamp](https://monosnap.com/file/A4sm9cDzuIVjfbFM0n1rb4QearZfx6.png "<[Source github](https://github.com/ChristopheDucamp)>")

### R1D1 : lundi 24 juillet

#### Comment j'ai Connu le Mouvement #100DaysOfCode

Tout simplement via une requête twitter "[#GoHugo](https://twitter.com/search?q=%23gohugo&src=typd)". Parachutage sur un post d'[Ivy DeWitt](https://twitter.com/zentechnista/status/889271653821296640) ("Pythonista" enthousiaste, newbie avancée en programmation et enthousiaste sur le défi) m'ayant conduit à lire attentivement son excellent article "[Lessons in Programming: Learning To Get Uncomfortable](https://zentechnista.github.io/2017/07/lessons-in-programming-learning-to-get-uncomfortable/)". Le reste n'est que promenade dans les hyperliens et tutoriel du freecodecamp.

#### Pourquoi je signe

Étant non développeur, j'essaye d'apprendre le code en amateur depuis quelques années. Après deux échecs sur des engagements pris début 2017 ([#100DaysOfPhotos](https://www.christopheducamp.com/2017/01/02/100daysofphoto-pourquoi/)...
et [résolutions indieweb 2017](https://indieweb.org/2017-01-01-commitments#Christophe_Ducamp)) et beaucoup de butinages amateurs dans le code pour essayer de suivre les  communautés [indieweb](https://indieweb.org) et [Jamstatic](https://jamstatic.fr/), j'aimerais à travers ce défi monter en compétences pour le plaisir d'apprendre de nouveaux métiers. Et imaginer parler plus proprement avec des développeurs.

Mes motivations essentielles pour rejoindre #100DaysOfCode sont donc par ordre de priorité :

1. **[Dogfooding](https://indieweb.org/dogfood-fr)** : monter en compétences sur le combo HTML/CSS sur mon site personnel.
2. **Rester concentré** et maintenir une routine pour rebondir sur mes engagements 2017. À savoir revoir de fond en comble mon vieux site web personnel (brisé à cette heure, motorisation Jekyll).
2. **M'imposer du temps** pour sortir de ma zone de confort. Faire mes premiers pas durant ce premier Round sur JavaScript et un langage de programmation (Golang ?) afin de mieux communiquer avec les devs des communautés indieweb et jamstatic.
3. **Pratiquer GitHub**. Etre à l'aise avec git, pratiquer les pull request, aider, collaborer. Bref *ne pas rester seul* dans l'effort.
4. Et pour finir une **motivation sociale**. Dans la vraie vie, je  vis à Paris et me sens prêt à aider et découvrir de nouveaux talents prêts à rejoindre le défi en langue française :)


#### Statut technique du jour :

Étude **[GoHugo](https://gohugo.io)** :
  lu et traduit une [première ébauche hugoDocs en français](https://github.com/ChristopheDucamp/hugoDocs-fr). Bataillé sans succès pour franciser la date des News dans les templates (fonctions héritées de Golang.) Trouvé une [solution à tester de francisation de date lisible pour les humains avec le suffixe 1er](https://discourse.gohugo.io/t/formatting-a-date-with-suffix-2nd/5701)

**Premiers pas sur Golang :**
variables d'environnement GOPATH et autres paramétrées dans mon profil bash. Prêt à jouer et apprendre. Découverte de l'éditeur WebStorm qui sait travailler en Golang avec une fenêtre de terminal intégré.

#### Production du jour

- GoHugo : [première ébauche de traduction du tutoriel Quick-Start GoHugo](https://github.com/ChristopheDucamp/hugoDocs-fr/blob/master/content/demarrage/quickstart.md). Il est testé et fonctionnel. À relire par les amis. Un output est à construire.
### R1D2 : mardi 25 juillet

Départ demain pour une semaine en Basse-Autriche. Prévoyant de travailler sans accès au réseau, j'ai repris les fondamentaux de Git pour prévoir de travailler "hors ligne".

Enregistré un compte sur freecodecamp et [parcouru les tutoriels sur les photos de chat](https://www.freecodecamp.org/challenges/create-a-set-of-checkboxes) jusqu'à l'étape 36.

Initialisé sur mon macbook 2 repos qui seront accessibles pour apprendre/coder/committer hors-ligne sur mon site personnel. (repos GolangTraining + HTML forkés chez Tod McLeod)

#### Production du jour

Pas de production aujourd'hui. Assimilé et révisé quelques fondamentaux git pour paramétrer, pousser et raffiner ce repo #100DaysOfCode (ébauche de traduction en français).

Encore désolé pour l'erreur de commit mal dirigé  sur le repo original.

Merci d'avoir lu et à demain.

[xtof_party](https://twitter.com/xtof_party)

![7 bonnes habitudes](https://monosnap.com/file/xKFYURjwzehl33RlFfmky8hyHrpwms.png)
### R1D3 : mercredi 26 juillet

Embarquement pour la Bassse-Autriche. Pas d'accès au réseau. Essayé sans succès quelques exercices à du <https://www.freecodecamp.org/challenges/> sur un téléphone.

#### Production : néant

### R1D4 : jeudi 27 juillet ([Sankt Pölten](https://fr.wikipedia.org/wiki/Sankt_P%C3%B6lten))


- Donnerstag 27 juli - organisation des dossiers
- Nettoyé le modèle "r1-log" en français
[source](https://github.com/Kallaway/100-days-of-code/edit/master/r1-log.md) pour le distinguer de mon journal personnel déposé sur un repo 100-days-of-code-xtof (contenu importé du "r1-log")
- groupe local statique [vienna.html](https://twitter.com/viennahtml)

#### Production

- déployé <https://100daysofcode.christopheducamp.com>.
- [bataille avec la francisation des dates](http://100daysofcode.christopheducamp.com/post/r1d4-100daysofcode/)


### R1D5 : vendredi 28 juillet
#### Progrès du jour :
- francisation de la date
<!--
`partials/post_meta.html`

```golang
<span class="post-meta">
Posté le <time class="post-date dt-published" datetime="{{ .Date.Format "2006-01-02T15:04:05Z07:00" | safeHTML }}">{{ .Date.Day }} {{ index $.Site.Data.mois (printf "%d" .Date.Month) }} {{ .Date.Year }}</time>
</span>
```

devrait rendre aujourdhui


    Posté le 28 juillet 2017
-->
- certificat https
- lien "améliorez cette page" sur les posts

### R1D6 : samedi 29 juillet

- bouton "améliorez cette page" sur les posts
- test galeries
- indieweb : web-signin

### R1D7 : dimanche 30 juillet

- indiemark niveau 1 - réglages de [h-entry](http://100daysofcode.christopheducamp.com/2017/07/30/r1d7-indiemark-niveau-1-3---posts---layout-list.html/)

### R1D8 : 31 juillet

- terminé le tutoriel bootstrap du freecodecamp
- découverte du défi de construction d'une page d'hommage

### R1D9 : révision HTML CSS
- ajouté shortcode `codepen`
- premiers pas sur la syntaxe emmet et raccourcis clavier webstorm
- révision box model
	- étude layout (`box-sizing: border-box`)

### R1D10 : fondamentaux CSS
- [révision sélecteurs CSS](https://100daysofcode.christopheducamp.com/2017/08/02/r1d10/) w Todd McLeod, un [instructeur recommandé](https://www.greatercommons.com/learn/6708511014649856) pour son intelligence et sa dextérité au clavier.


### R1D11 : fondamentaux CSS 
- Configuration IDEs pour CSS (Atom et Webstorm. Lequel choisir ?)
- Spécificité CSS : utilisation du **[Calculateur Spécifité CSS](https://specificity.keegan.st/)** pour déterminer quel élément sera appliqué : 
	1. style dans la ligne - 1000
	2. id - 100
	3. classe, attribut, pseudo-classe - 10
	4. élément, pseudo-élément - 1
- exploration [propriété-raccourcie `font](https://developer.mozilla.org/fr/docs/Web/CSS/font)


### R1D12 : 4 août - HTML framework bootstrap
- [Défi freecodecamp : Build a Tribute Page](https://www.freecodecamp.org/challenges/build-a-tribute-page). Dépôt HTML à raffiner sur <https://codepen.io/xtof-party/details/prNRra/> (bootstrap)

### R1D13 5 août cours OpenClassroom bootstrap

- Achevé la partie 1 [Premiers Pas](https://openclassrooms.com/courses/prenez-en-main-bootstrap)

### R1D14 6 août cours Todd McLeod Flexbox 

- lien de travail <https://github.com/GoesToEleven/html-css-bootcamp/tree/master/031_flexbox>

### R1D15 - 7 août - Flexbox et MAJ Hugo
- Fait [14 pages d'exercices par Todd McLeod](https://github.com/GoesToEleven/html-css-bootcamp/tree/master/031_flexbox/03_hands-on-exercises/01_challenges) et joué avec [Flexbox Froggy](http://flexboxfroggy.com/#fr).
- Mise à jour motorisation  [Hugo 0.26.](https://gohugo.io/news/0.26-relnotes/). Modifié `config.toml` pour activer les "guillemets en français".

### R1D16 - 8 août - étude design "flexbox" 
Pas de production.
- Révision des "Media Queries"
- Flexbox : exercices sur le [modèle de design flexbox proposé par Google](https://developers.google.com/web/fundamentals/design-and-ui/responsive/patterns)

### R1D17 - 9 août

- Révision layout CSS
- Apprentissage JavaScript / [freecodecamp](https://www.freecodecamp.org/)
- Achevé le cours [Git,Github sur Openclassrooms](https://openclassrooms.com/courses/gerer-son-code-avec-git-et-github). 

### R1D18 - 10 août 

- ébauche layout "above-the-fold"

### R1D9 - 11 août 

- layout html/css background full page responsive

### R1D20 - 12 août 

- étude viewport 
- en-tête de layout pleine page responsive 
	- essais icônes svg 