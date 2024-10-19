 Projet Maven de Gestion de Salles et de Machines

Ce projet Maven est une application Java qui gère des entités de type **Salle** et **Machine**. Il utilise Hibernate pour la persistance des données et suit le modèle DAO (Data Access Object) pour interagir avec la base de données.

Table des matières

- [Fonctionnalités](#fonctionnalités)
- [Technologies utilisées](#technologies-utilisées)
- [Structure du projet](#structure-du-projet)
- [Configuration](#configuration)
- [Exécution](#exécution)
- [Tests](#tests)
- [Contributeurs](#contributeurs)
- [Licence](#licence)

 Fonctionnalités

- Gestion des salles : création, mise à jour, suppression et recherche de salles.
- Gestion des machines : ajout, modification, suppression et recherche de machines.
- Utilisation de DAO pour séparer la logique d'accès aux données de la logique métier.

 Technologies utilisées

- Java 8
- Maven pour la gestion des dépendances.
- Hibernate pour la gestion de la persistance des données.
- MySQL comme base de données.
- JUnit pour les tests unitaires.
  
 Description des classes

- entities.Machine
  - Représente une machine avec des attributs tels que `reference`, `dateAchat`, et une référence à une salle.
  
- entities.Salle
  - Représente une salle avec un attribut `code` et une collection de machines associées.

- services.MachineService
  - Classe de service pour gérer les opérations sur les machines, implémente `IDAO`.

- services.SalleService
  - Classe de service pour gérer les opérations sur les salles, implémente `IDAO`.
