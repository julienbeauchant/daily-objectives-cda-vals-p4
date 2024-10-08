# Objectifs journaliers

### Mercredi 18/09/2024 :

- [ ] Faire le wargame bandit jusqu'au niveau 5 (anglais)

Seulement si le wargame bandit est au niveau 5 minimum :

#### Git

- [x] Création de compte + configuration Github
- [x] Installation et configuration de Git
- [x] Comprendre le versionning
<!-- le versionning permet de sauvgarder au fur et à mesure son projet 
tout en gardant une trace des anciennes sauvegardes en cas de besoin -->
- [ ] Comprendre le fonctionnement de Git
<!-- git utilise le versionning -->
  - [ ] Comprendre le staging de Git
  - [x] Comprendre le fonctionnent et l'utilité des commandes de bases de Git :
    - [x] git init
    <!-- permet d'initialiser un dépôt git -->
    - [x] git clone
    <!-- permet de cloner/duppliquer un projet sur le local -->
    - [x] git status
    <!-- permet de savoir quelles modifications sont en cours -->
    - [x] git pull
    <!-- permet de récupérer les modifications apportées au fichier -->
    - [x] staging area
    <!-- zone intermédiaire pour préparer les modifications avant de les enregistrer -->
    - [x] git add
    <!-- permet d'ajouter les modifications du fichier dans le staging area  -->
    - [x] git commit
    <!-- permet d'enregistrer les modifications ajoutées au staging area après un git add -->
    - [x] git push
    <!-- permet d'envoyer les modifications au fichier -->
    - [x] git remote
    <!-- permet de gérer les connexions entre le dépôt local et les dépôt distants -->
    - [x] git merge
    <!-- permet de combiner les modifications de branches dans le dépôt local -->

- [ ] Faire le parcours Git-it pour les débutants (Nodeschool.io)
- [x] Faire ses premiers commits sur les daily objectives
- [x] Faire ses premiers pushs des daily-objectives sur son compte Github
- [x] Faire ses première manipulations de versionning en CLI only (init, push, add, commit, status, pull)

* [x] Comprendre les termes "local", "origin", "main" et "upstream"
  <!-- local signifit ma machine -->
  <!-- origin est le nom utilisé pour faire référence au dépôt distant principal associé à mon dépot local -->
  <!-- main est la branche principale d'un dépot -->
  <!-- pour le cas du fork, upstream est le dépot d'origine qui a été forké -->
* [x] Faire ses premiers commits sur les daily objectives (plusieurs commits par jour pour les débutants)
* [x] Faire ses premiers pushs des daily-objectives sur son compte Github
* [ ] Découvrir les conventions de nommage de son versionning avec la convention Angular :
  - [ ] https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format
  - [ ] https://www.conventionalcommits.org/fr/v1.0.0/
  - [ ] Renommer son dernier commit en respectant cette convention
* [x] Comprendre le fonctionnement des branches dans Git :
<!-- les branches ne sont pas créees pour une personne mais plutôt pour une fonctionnalité -->
  - [x] Lister, changer, créer, supprimer des branches
  <!-- lister les branches local : git branch -->
  <!-- changer de branche : git switch nom-de-la-branche -->
  <!-- créer une branche : git branch nom-de-la-branche -->
  <!-- supprimer une branche : 
    - si la branche a été fusionnée et donc sans perdre les modifications : git branch -d nom-de-la-branche
    - si la branche n'a pas été fusionnée et donc sans garder les modifications : git branch -D nom-de-la-branche  -->
  - [x] Quelle est la différence entre `Git switch` et `Git checkout`
  <!-- git switch permet de changer de branche -->
  <!-- git checkout permet de créer et changer de branche  -->
  <!-- switch sera préféré car son action et simple et clair alors que checkout est plus confut car plusieurs usages  -->
* [x] Comprendre le merge dans Git
<!-- le merge est le fait de fusionner -->
  - [ ] Comprendre le "fast forward"
  <!-- le fast forward signifit un bon sur un commit -->
  - [x] Quelle est la différence entre un "commit" et un "merge commit" ?
  <!-- un commit est un enregistrement instantané du projet -->
  <!-- un merge commit enregistre l'intégration des modifications de branches lorsque celles-ci fusionnent et ( créer un nouveau commit ) ( merge ) -->

#### Github

- [ ] Pimper son profile Github (belle du village)
- [x] Configurer un tunnel SSH entre son local et son Github
- [ ] Découvrir l'interface de Github :
  - [x] Pull Requests
  <!-- c'est une demande pour que des modifications effectuées sur une branche soient intégrées dans une autre, à savoir que les commit d'une branche restent en mémoire et même après la fusion -->
  - [x] Branches
  <!-- le système de branches permet de travailler sur un même projet mais séparemment -->
  - [ ] Issues
  - [ ] Settings projet
  - [ ] Settings profile

  <!-- git est rapide car il enregistre que les modifications apportées au projet au lieu de recréer complétement le fichier -->
