# Objectifs journaliers

## Lundi 18/11/2024 :

### MERISE - Le MLD (Modèle Logique de Données)

- [ ] Passage du MCD au MLD
  - [ ] Savoir appliquer les règles de passage
    - Les entités deviennent des tables.
    - les associations peuvent devenir des tables ou une contraite relationnelle.
    - Les attributs des entités et associations deviennent des colonnes.
    - Les identifiants uniques deviennent des clés primaires.
  - [ ] Savoir gérer les relations **1:1**
    - Ajout d'une clé étrangère dans l'une des deux tables.
  - [ ] Savoir gérer les relations **1:N**
    - Clé étrangère dans la table correspondant à l’entité du côté N.
  - [ ] Savoir gérer les relations **N:M**
    - Table intermédiaire contenant les clés primaires des deux entités impliquées dans la relation.
  - [ ] Savoir gérer les contraintes d'intégrité
    - [ ] Clés primaires
      - Chaque table doit avoir une clé primaire.
    - [ ] Clés étrangères
      - Les clés étrangères servent à établir les relations entre les tables.
      - Une clé étrangère doit pointer vers une clé primaire d’une autre table.
    - [ ] Contraintes d'unicité
      - Certains attributs doivent être uniques dans une table, même si ils ne sont pas des clés primaires.