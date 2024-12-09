# Objectifs journaliers

## Lundi 09/12/2024 :

### Programmation Orientée Objet - Concepts avancés
<hr>

- [ ] Étudier le concept d'héritage
<br>

  - **Héritage :** *Concept qui permet à une classe (classe enfant ou sous-classe) d’hériter des attributs et des méthodes d’une autre classe (classe parent ou super-classe)*
<br>

  - [ ] Fonctionnement du mode parent/enfant
<br>

  - **Classe parent :** *Définit des attributs et des méthodes qui seront communs à toutes ses classe enfant / sous-classes.*
<br>

  - **Classe enfant :** *Hérite des attributs et des méthodes du parent, mais peut également :*
<br>
    - **Étendre** *le parent en ajoutant de nouveaux attributs ou de nouvelles méthodes*
    - **Redéfinir** *les méthodes héritées pour les adapter*
<br>

- [ ] Utilisation du mot clé super
<br>

  - **Super :** *Ce mot-clé permet d'appeler une méthode du parent si elle est redéfinie dans l'enfant.  
  Il est également utilisé pour appeler le constructeur du parent pour initialiser les attributs hérités*
<br>

- [ ] Fonctionnalités étendues entre un parent et un enfant
  - [ ] Analyse du concept de polymorphisme
<br>

  - **Polymorphisme :** *Capacité d’un objet à prendre plusieurs formes.  
  Cela permet d’utiliser des méthodes de manière générique, même si leur comportement diffère selon la classe qui les implémente ou les redéfinit*
<br>

- [ ] Méthode commune
<br>

  - **Redéfinition :** *Une sous-classe peut redéfinir une méthode héritée du parent avec le même nom, le même type de retour et les mêmes paramètres*
<br>

  - **Override :** *Une classe enfant peut redéfinir une méthode héritée du parent pour en modifier le comportement.  
  Lorsqu’une méthode redéfinie est appelée via une référence du type parent, le comportement de la classe enfant sera exécuté*

<br>

  - [ ] Surcharge
<br>

  - **Surcharge :** *Consiste à définir plusieurs méthodes avec le même nom mais des signatures différentes (différents types ou nombre de paramètres) dans la même classe*
<br>

- [ ] Apprentissage des relations possibles entre les classes
<br>

  - [ ] **Association :** *Relation entre deux classes où une classe utilise / ou est liée à une autre.  
  Elle indique qu’il existe une dépendance logique ou une connexion entre les objets des deux classes, mais sans notion de propriété stricte*
<br>

  - [ ] **Agrégation :** *Type particulier d’association où une classe possède une relation avec une autre classe, mais celles-ci peuvent exister indépendamment des autres*
<br>

  - [ ] **Composition :** *Forme plus forte d’agrégation où une classe possède d'autres classes qui ne peuvent pas exister indépendamment.  
  Si l’objet de cette classes est détruit, alors les autres classes le sont aussi*
<br>

<hr>

#### Résumé :

  - **Héritage :** *Relation parent-enfant où l’enfant hérite des attributs et méthodes du parent*
<br>  

  - **Super :** *Mot-clé pour accéder aux membres ou au constructeur du parent*
<br>  

  - **Redéfinition (Override) :** *La sous-classe modifie une méthode héritée pour lui donner un comportement spécifique*
<br>  

  - **Surcharge (Overloading) :** *Une classe définit plusieurs méthodes avec le même nom mais des signatures différentes*
<br>  

  - **Polymorphisme :** *Permet de manipuler les objets de manière générique via des références de type parent tout en exécutant le comportement spécifique des objets enfants*
<br>  

  - **Association :** *Lien général entre deux classes sans notion de propriété*
<br>  

  - **Agrégation :** *Relation “partie-tout” où les parties peuvent exister indépendamment du tout* 
<br>  

  - **Composition :** *Relation “partie-tout” où les parties sont détruites en même temps que le tout*
<br>   