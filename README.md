# Compte Rendu 
# E-banking app

## Author

- [Aya Zouity](https://github.com/Ayaytiuoz)

## Plan
- Le contexte generale de l'application
- diagramme de classe 
- Architecture du Projet
- Interface Graphique
- conclusion

## Le contexte generale de l'application
Notre application d'e-banking offre une gestion pratique et sécurisée des comptes bancaires en ligne pour les administrateurs. Elle repose sur une architecture multicouche bien structurée, combinant des technologies telles que Spring MVC pour le backend et Angular pour le frontend.

Du côté backend, nous avons développé des fonctionnalités essentielles. Les administrateurs peuvent créer de nouveaux clients, ouvrir différents types de comptes bancaires tels que les comptes d'épargne et les comptes courants, et gérer les opérations financières telles que les débits, les crédits et les transferts d'argent entre les comptes. Nous avons accordé une attention particulière à la sécurité et à la fiabilité de ces fonctionnalités.

En ce qui concerne le frontend, nous avons mis en place une interface utilisateur conviviale en utilisant Angular. Cette interface permet aux administrateurs de rechercher facilement des clients, d'afficher les informations relatives aux comptes et d'effectuer des opérations financières de manière intuitive. Nous avons accordé une grande importance à l'expérience utilisateur, en veillant à ce que l'application soit facile à naviguer et à utiliser.

Tout au long du processus de développement, nous avons consacré du temps à la conception, au développement et aux tests de chaque fonctionnalité. Nous avons veillé à ce que notre application d'e-banking soit complète, fiable et réponde aux besoins des administrateurs en matière de gestion des comptes bancaires en ligne.

## diagramme de classe

![App Screenshot](/interface/page.png)
## Architecture du Projet
### Architecture du Backend:

Dans notre application Spring MVC, nous avons adopté une architecture multicouche courante pour le backend. Voici un aperçu des principales couches de notre architecture :

#### Couche de Présentation (Presentation Layer) :
Cette couche gère les requêtes HTTP entrantes et les réponses sortantes. Nous avons utilisé des contrôleurs REST pour recevoir les requêtes provenant du frontend et renvoyer les réponses appropriées. Les contrôleurs REST assurent la coordination entre les différentes couches de l'application.

#### Couche de Service (Service Layer) :
La couche de service contient la logique métier de notre application. Elle traite les requêtes reçues des contrôleurs REST, effectue les opérations nécessaires, utilise les entités et les DTO (Data Transfer Objects) pour manipuler les données, et renvoie les résultats aux contrôleurs. Cette couche encapsule la logique métier et favorise la réutilisabilité du code.

#### Couche d'Accès aux Données (Data Access Layer) :
Cette couche gère l'accès aux données persistantes, généralement stockées dans une base de données. Nous avons utilisé des repositories pour interagir avec la base de données. Les repositories offrent des méthodes permettant d'effectuer des opérations CRUD (Create, Read, Update, Delete) sur les entités de notre application. Ils fournissent une abstraction pour accéder et manipuler les données de manière efficace.

#### Couche de Mappage (Mapping Layer) :
Cette couche est responsable de la conversion des objets entre les entités et les DTO. Nous avons utilisé des bibliothèques de mappage telles que ModelMapper ou MapStruct pour faciliter cette conversion. Cela permet de transférer les données entre les différentes couches de l'application tout en maintenant une séparation claire entre les entités de la base de données et les objets utilisés dans la couche de présentation.

### Architecture du Frontend :

Dans notre application Angular, nous avons suivi une architecture courante pour le frontend, en utilisant les éléments suivants :

#### Composants (Components) :

Les composants sont les éléments de base de l'interface utilisateur. Chaque composant représente une partie spécifique de l'interface et contient la logique nécessaire pour interagir avec les utilisateurs. Les composants encapsulent le HTML, le CSS et la logique associée à une partie spécifique de l'application.

#### Services :
Les services sont responsables de la gestion de la logique métier côté client. Ils communiquent avec le backend en effectuant des appels HTTP pour récupérer les données nécessaires et effectuer des opérations. Les services fournissent des fonctionnalités réutilisables et permettent de séparer la logique de présentation des composants.

#### Modèles et Directives :
Les modèles Angular définissent la structure de l'interface utilisateur en utilisant une syntaxe basée sur HTML. Les directives sont utilisées pour ajouter des fonctionnalités et interagir avec les composants. Elles permettent de manipuler dynamiquement le DOM, d'afficher des données conditionnellement et de réagir aux événements de l'utilisateur.

#### Routage (Routing) :
Angular offre un système de routage qui permet de gérer la navigation entre différentes pages et vues de l'application. Le routage permet de définir des routes pour chaque vue et de contrôler dynamiquement l'affichage des composants en fonction de l'URL actuelle.

#### Module HTTP :
Angular fournit un module HTTP qui facilite les requêtes HTTP vers le backend. Il permet d'interagir avec les API REST, d'envoyer des requêtes, de traiter les réponses et de gérer les erreurs.

## Interface Graphique

#### Notre application e-banking propose une interface de recherche et d'affichage des clients, offrant aux administrateurs une manière conviviale et intuitive de trouver rapidement les informations relatives à un client spécifique.
![App Screenshot](/interface/page1.png)
![App Screenshot](/interface/page11.png)
#### L'interface d'ajout d'un client dans notre application e-banking offre aux utilisateurs un formulaire clair et intuitif, facilitant la saisie des informations nécessaires pour créer un nouveau compte client.
![App Screenshot](/interface/page2.png)
#### L'interface des opérations bancaires dans notre application e-banking permet aux utilisateurs de consulter les opérations associées à un compte spécifique et d'effectuer de nouvelles opérations.
![App Screenshot](/interface/page3.png)
#### L'interface "Customer Accounts" dans notre application e-banking permet aux utilisateurs de visualiser la liste des comptes associés à un client spécifique, en utilisant une pagination pour faciliter la navigation.
![App Screenshot](/interface/page4.png)
#### La page "New Account" de notre application e-banking permet aux utilisateurs de créer facilement un nouveau compte bancaire pour un client existant.
![App Screenshot](/interface/page5.png)
## Conclusion

Cette application de gestion des comptes bancaires offre une solution pratique et efficace pour les utilisateurs, prenant en charge les opérations de débit et de crédit. Chaque compte est attribué à un client et propose des options de compte courant et d'épargne. Elle améliore la gestion financière personnelle, facilite les transactions bancaires et favorise une meilleure organisation des fonds. Avec sa conception sécurisée, cette application constitue un outil précieux pour les individus cherchant à optimiser leur expérience bancaire et à développer des habitudes d'épargne solides.