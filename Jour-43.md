# Objectifs journaliers

## Vendredi 15/11/2024 :

### MERISE - Normalisation et dépendances fonctionnelles

- [ ] Introduction à la normalisation
  - **Qu'est-ce que la normalisation ? :**
    - Processus qui consiste à organiser les données dans une base de données pour éviter les redondances et les anomalies de mise à jour, d’insertion et de suppression.
  - **Quelles sont les différentes étapes de la normalisation ? :**
    - Les différentes étapes s'appellent les formes normales (FN ou NF).
  - [ ] Comprendre l'importance de la normalisation
    - La normalisation est importante pour éviter les redondances, les anomalies de mise à jour, d’insertion et de suppression.
  - [ ] Savoir identifier les anomalies de redondance
<br>
- [ ] Les formes normales
  - **Les formes normales fonctionnent pas étapes, une étape ne peut pas commencer si la précédente n'a pas été faite.**
  - [ ] Comprendre la 1ère forme normale (1FN)
    - **1NF :** La 1ère forme normale conciste à garantir que les données des attributs soit atomique et indivisible.  
    **Exemple :** faire une colonne distincte entre nom et prénom.
  - [ ] Comprendre la 2ème forme normale (2FN)
  **"un attribut non identifiant ne depend pas d'une partie de l'identifiant mais de tout l'identifiant".**
    - **2NF :** La 2ème forme normale consiste à spliter les attributs qui dépendent partiellement de l'identifiant (clé). 
  - [ ] Comprendre la 3ème forme normale (3FN)
  **"un attribut non identifiant ne depend pas d'un ou plusieurs attributs non-clé."**  
    - **3NF :** La 3ème forme normale consiste à ce que tous les attributs dépendents inuquement et directement de l'identifiant (clé).
<br>
- [ ] Les dépendances fonctionnelles
  - [ ] Savoir identifier les DF élémentaires
  - [ ] Savoir identifier les DF composées
  - [ ] Savoir identifier les DF transitives
