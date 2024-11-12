# Objectifs journaliers

## Mercredi 30/10/2024 :

### Introduction à PostgreSQL et DCL

- [ ] Découverte de PostgreSQL
  - [ ] Identifier les différences entre MySQL et PostgreSQL
  <!-- SGBDR = système de gestion de base de données relationnelle -->
    - MySQL est une base de données relationnelle
    - PostgreSQL est une base de données relationnelle objet
  - [ ] Savoir Expliquer les avantages de PostgreSQL
  - [ ] Savoir Choisir les cas d'usage adaptés à PostgreSQL

- [ ] Installation et Configuration
  - [ ] Installation de PostgreSQL sur la machine
    - sur Mac via Homebrew : brew install postgresql
  - [ ] Installation de pgAdmin
    - sur Mac via Homebrew : brew install --cask pgadmin4
  - [ ] Installation de pgcli
    - sur Mac via Homebrew : brew install pgcli
    - activier pgcli : pgcli postgres 
    - connexion à la bdd avec pgcli : pgcli -U utilisateur -d nom-database
    - deconnexion de la bdd avec pgcli : \q
  - [ ] Configuration initiale
    - vérifie que postgresql est bien installé : psql --version ou postgres --version
    - démarrer le serveur postgresql : brew services start postgresql@14 (@14 étant la version)
    - arrête le service postgresql : brew services stop postgresql@14
    - redemarrer le service postgresql : brew services restart postgresql@14
    - vérifie dans hombrew ce qui est en cours d'exécution : brew services list
    - vérifie que le serveur postgresql est en cours d'exécution : pg_isready
    - [ ] Ports
    - [ ] Mot de passe postgres
    - [ ] Création du premier utilisateur
  - [ ] Test de la connexion

- [ ] Data Control Language (DCL)
  - [ ] Gestion des utilisateurs
    - [ ] Savoir construire des requêtes CREATE USER
    - [ ] Savoir modifier des utilisateurs avec ALTER USER
      - modifie un rôle dans la bdd
    - [ ] Savoir supprimer des utilisateurs avec DROP USER
      - supprimer un rôle de la bdd
    - [ ] Savoir utiliser les rôles PostgreSQL
  
  - [ ] Gestion des droits
    - [ ] Savoir attribuer des privilèges avec GRANT
      - [ ] Droits sur les bases de données
      - [ ] Droits sur les tables
      - [ ] Droits sur les colonnes
    - [ ] Gérer la révocation avec REVOKE
      - [ ] Comment retirer des droits sur une base de données, une table ou une colonne ?
      - [ ] Quel est l'impact d'une révocation en cascade ?
        - la suppression de toutes les données de la bbd 

  - [ ] Les bonnes pratiques de sécurité
    - [ ] Comment appliquer le principe du moindre privilège dans PostgreSQL ?
      - en attribuant des rôles
      - en limitant les accès selon les users ou les rôles
    - [ ] Quand utiliser des rôles plutôt que des utilisateurs individuels ?
      - plus judicieux d'utiliser des rôles lorsque plusieurs users ont les mêmes privilèges ou accès
      - utiliser des users individuels lorsque les besoins sont spécifiques
    - [ ] Comment auditer efficacement les droits d'accès ?