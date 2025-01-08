# Objectifs journaliers

## Vendredi 13/12/2024 :

### UML - Diagrammes de cas d'utilisation et diagramme de classes
<hr>

- [ ] Faire les objectifs de la veille
<br>

- [ ] Découverte avancé des cas d'utilisation (Use Case Diagram) (les relations)
<br>
- Le diagramme de cas d'utilisation illustre les interactions entre des acteurs et le système que l’on modélise.  
  Il montre les fonctionnalités ou services offerts par le système d’un point de vue utilisateur, sans entrer dans les détails techniques.
<br>

- [ ] Comprendre la notion d'association
<br>

L’association est une relation simple entre un acteur et un cas d’utilisation
  - Elle indique que l’acteur participe activement à la réalisation du cas d’utilisation
  - Représentée par une ligne pleine entre l’acteur et le cas d’utilisation

**Exemple :**  
    Un acteur “Client” est associé au cas d’utilisation “Passer une commande”. Cela signifie que le client initie ou participe à cette fonctionnalité
<br>

  - [ ] Comprendre et représenter le terme d'inclusion
    - L’inclusion est une relation obligatoire entre deux cas d’utilisation
      - Elle indique qu’un cas d’utilisation inclut systématiquement un autre cas d’utilisation dans son déroulement
      - Représentée par une flèche en pointillés avec le mot-clé "include"
    - **Objectif :**
      - Réutilisation : Permet de décomposer un processus en sous-processus réutilisables
      - L’inclusion représente une dépendance fonctionnelle stricte
    - **Exemple :**
    Cas d’utilisation “Passer une commande” inclut “Vérifier la disponibilité du produit”  
    Cela signifie que chaque fois qu’une commande est passée, le système vérifie si le produit est disponible
<br>
  - [ ] Comprendre et représenter le terme d'extension
    - L’extension est une relation optionnelle entre deux cas d’utilisation
      - Elle indique qu’un cas d’utilisation peut être étendu par un autre dans certaines conditions
      - Représentée par une flèche en pointillés avec le mot-clé "extend"
    - **Objectif :**
      - Décrire des comportements supplémentaires ou exceptionnels déclenchés par des conditions spécifiques
      - L’extension permet de modéliser des variations ou des cas d’exception sans surcharger le cas d’utilisation principal
    - **Exemple :**
    Cas d’utilisation “Passer une commande” peut être étendu par “Appliquer un code de réduction” si le client entre un code promo
<br>
  - [ ] Comprendre et représenter la généralisation
    - La généralisation est une relation hiérarchique entre deux cas d’utilisation ou deux acteurs
      - Elle indique qu’un cas d’utilisation spécifique ou un acteur spécifique hérite du comportement d’un cas ou d’un acteur plus général
      - Représentée par une flèche pleine avec une pointe creuse
    - **Objectif :**
      - Représenter des variantes spécialisées d’un cas d’utilisation ou d’un acteur
    - **Exemple pour les cas d’utilisation :**
      - Cas d’utilisation général : “Payer une commande”
      - Cas spécialisés : “Payer par carte bancaire” et “Payer par PayPal”
        - Ces cas spécialisés héritent du comportement général tout en ajoutant des particularités
    - **Exemple pour les acteurs :**
      - Acteur général : “Utilisateur”
      - Acteurs spécialisés : “Client” et “Administrateur”
        - Le “Client” et l’“Administrateur” héritent des interactions communes de l’“Utilisateur”, mais possèdent des rôles spécifiques
<br>
- [ ] Découverte du diagramme de classes
  - Le diagramme de classes est l’un des diagrammes structurels les plus fondamentaux en UML.
Il représente la structure statique d’un système en modélisant ses classes, leurs attributs, leurs méthodes et leurs relations (associations, dépendances, généralisations, etc.). Il permet de visualiser comment les entités du système sont organisées et reliées entre elles
<br>
  - [ ] Etude générale du diagramme de classes
    - [ ] Objectifs
      - **Modéliser la structure du système :**
      Fournir une vue d’ensemble des entités principales et de leurs relations
      - **Conceptualiser un domaine métier :**
      Définir les concepts du domaine d’application (ex. clients, produits, commandes)
      - **Concevoir et documenter l’architecture logicielle :**
      Spécifier les classes, interfaces, attributs et méthodes pour le développement
      - **Favoriser la réutilisabilité et la maintenabilité :**
      Identifier les composants réutilisables, les relations de hiérarchie (héritage), et les dépendances
      - **Servir de base pour d’autres diagrammes :**
      Les diagrammes dynamiques (séquence, communication) utilisent les classes définies dans ce diagramme
<br>
	- [ ] Dans quels cas est-il utilisé ?
    - **Phase de conception :**
      - Pour structurer et planifier l’architecture logicielle
      - Pendant la conception d’une base de données relationnelle
    - **Analyse des besoins :**
      - Pour modéliser les concepts métier ou les entités importantes d’un système
    - **Documentation technique :**
      - Pour expliquer et transmettre la structure du système aux développeurs ou aux parties prenantes
    - **Refactoring ou extension :**
      - Pour analyser et améliorer une architecture existante
<br>
  - [ ] Etudier la représentation d'une classes
    - Une classe est représentée par un rectangle divisé en trois sections
    - [ ] Son formalisme
      - **Nom de la classe :**
      Obligatoire. Écrit en haut, avec un éventuel stéréotype (ex. "interface").
	- [ ] **Les attributs :** 
    - Représentent les propriétés ou caractéristiques de la classe
    - Écrits sous la section “Attributs”, précédés de leur visibilité
	- [ ] Les méthodes
    - Représentent les comportements ou les fonctions de la classe
    - Écrites sous la section “Méthodes”, précédées de leur visibilité
	- [ ] L'encapsulation
    - Les niveaux de visibilité (encapsulation) spécifient comment les attributs ou méthodes peuvent être accessibles :
    : + (public) : Accessible partout
    : # (protected) : Accessible par la classe elle-même et ses sous-classes
    : - (private) : Accessible uniquement dans la classe
    : ~ (package) : Accessible par toutes les classes du même package
  - L’encapsulation permet de contrôler l’accès aux données (attributs) pour assurer la cohérence et protéger l’intégrité des objets
<br> 
  - [ ] Etudier les différences avec le MCD de la méthode MERISE
  
- [ ] Cas pratique
  - [ ] Réaliser le diagramme de cas d'utilisation d'une société de réservation de taxis
  - [ ] Réaliser le diagramme de classes d'une bibliothèque

**Exemple complet d’un diagramme de cas d’utilisation :**

Contexte : Système de commande en ligne
  - Acteurs :
    - “Client” (acteur principal).
    - “Administrateur” (acteur secondaire).
  - Cas d’utilisation principaux :
    - “Passer une commande”.
    - “Gérer les produits” (pour l’administrateur).
  - Relations :
    - “Passer une commande” inclut “Vérifier la disponibilité du produit”.
    - “Passer une commande” peut être étendu par “Appliquer un code de réduction”.
    - “Payer une commande” est un cas d’utilisation généralisé, avec deux variantes : “Payer par carte bancaire” et “Payer par PayPal”.

**Pourquoi utiliser un diagramme de cas d’utilisation ?**
  - Simplicité :
    - Facile à comprendre pour les parties prenantes non techniques.
  - Focus utilisateur :
    - Se concentre sur les besoins des utilisateurs et leurs interactions avec le système.
  - Complémentarité :
    - Sert de point de départ pour détailler d’autres diagrammes UML (séquence, activités, etc.).

En résumé, le diagramme de cas d’utilisation est essentiel pour capter et modéliser les attentes des utilisateurs et structurer les fonctionnalités de manière claire.

Définition des attributs et méthodes

Attributs :

Les attributs sont les propriétés ou les données membres de la classe. Chaque attribut est défini par :
  - Un nom : Identifiant de l’attribut.
  - Une visibilité (+, #, -, ~).
  - Un type : Précise la nature de la donnée (ex. int, String).
  - Une valeur par défaut (optionnelle)
  - Une multiplicité (optionnelle) : Définit combien de valeurs l’attribut peut contenir (ex. [1], [0..*]).

Méthodes (ou opérations) :

Les méthodes définissent les comportements d’une classe. Une méthode est caractérisée par :
  - Un nom
  - Une visibilité (+, #, -, ~)
  - Une liste de paramètres (nom et type)
  - Un type de retour.

Relations entre classes
1.  **Association :**
    - Relation logique entre deux classes (ex. “Un étudiant est inscrit dans un cours”)
    - Peut avoir une multiplicité (ex. 1 étudiant pour plusieurs cours) et une direction (bidirectionnelle ou unidirectionnelle).
2.  **Dépendance :**
    - Une classe dépend d’une autre pour fonctionner (ex. un paramètre d’une méthode).
3.	**Généralisation :**
    - Représente une relation d’héritage ou de spécialisation (ex. “Une voiture est un véhicule”).
4.	**Composition :**
    - Relation forte où une classe fait partie intégrante d’une autre (ex. “Un moteur appartient à une voiture”).
    - Représentée par un losange noir
5.	**Agrégation :**
    - Relation faible où une classe est liée à une autre (ex. “Un étudiant fait partie d’un groupe”)
    - Représentée par un losange blanc.

Exemple complet d’un diagramme de classes

Contexte : Gestion d’un système de bibliothèque  
  - Classe Livre :
    - Attributs :
      - titre : String
      - auteur : String
      - isbn : String
- Méthodes :
  + emprunter() : void
  + retourner() : void
- Classe Membre :
  - Attributs :
    - nom : String
    - id : int
    - livresEmpruntes : Livre [0..*]
- Méthodes :
  + inscrire() : void
  + emprunterLivre(livre : Livre) : void
  + rendreLivre(livre : Livre) : void
- Classe Bibliotheque :
  - Attributs :
    - nom : String
    - livres : Livre [0..*]
    - membres : Membre [0..*]
- Méthodes :
  + ajouterLivre(livre : Livre) : void
  + inscrireMembre(membre : Membre) : void

Relations :  
  - Une composition entre Bibliotheque et Livre (les livres appartiennent à la bibliothèque).  
  - Une association entre Membre et Livre (un membre peut emprunter plusieurs livres).

### Conclusion  

Le diagramme de classes est un outil fondamental pour structurer un système et organiser ses entités.  
Avec son focus sur les attributs, méthodes et relations, il permet une modélisation claire et une documentation précise, facilitant le développement et la communication entre équipes techniques et métiers