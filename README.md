## Tableau du lexique

### ARCHITECTURE

| Terme technique  | Définition & différence si besoin |
| - | - |
| Design pattern | **Un design pattern (= patron de conception) est une façon standardisée de résoudre un problème de conception logiciel récurrent.** Le design pattern décrit les grandes lignes d'une solution qui peuvent ensuite être modifiées et adaptées en fonction des besoins. Ca va de "copier-coller stackoverflow et adapter à son propre code" à l'idée de "factory en POO - une logique commune à tous les objets qui en sortent" |
| MVC | **Le MVC est un modèle architectural qui sépare la logique d'une application en trois composants ayant chacun des responsabilités différentes** : Un modèle (*Model*) contient les données à afficher (objets à manipuler...). Une vue (*View*) contient la présentation de l'interface graphique. Un contrôleur (*Controller*) contient la logique concernant les actions effectuées par l'utilisateur (gère l'aspect dynamique: Get, Post...). Intéret: SOC, DRY (un model pour plusieurs views...), modularité (changer que les views pour changer l'affichage) ![image](https://user-images.githubusercontent.com/75088424/123945545-90a93300-d99e-11eb-899e-21f0e87dcf69.png)|
| Architecture | **L’architecture d’un logiciel décrit la manière dont sont agencés les différents éléments d’une application et comment ils interagissent entre eux.** La conception de l’architecture conditionne la stabilité, l'efficacité et la pérennité du développement d'un logiciel. Une bonne architecture est évolutive, simple, maintenable (avec des outils pour la maintenance, TDD?), compatible (marche sur tous les OS, responsive...), interconnectée (avec d'autres systèmes d'information...)|

### BACK

| Terme technique  | Définition & différence si besoin |
| - | - |
| API | *Application Programming Interface (= interface de programmation d'application)*. **Une API permet à deux applications de communiquer entre elles. Elle permet d'*exposer*, de rendre disponibles les données ou les fonctionnalités d’une application existante afin que d’autres applications les utilisent.** C'est une interface, un peu comme la carte du menu entre la cuisine et mon assiette. Les API permettent aux développeurs de gagner du temps en profitant de la mise en œuvre d’une plate-forme pour faire le travail de fond. Cela permet de réduire la quantité de code qu'ils doivent créer, et contribue également à créer plus de cohérence entre les applications pour une même plateforme. (ex: une API pour capturer des photos à partir de la caméra du téléphone mobile - on ne code pas l'appel à la caméra...)|
| API REST | *Representational State Transfer Application Program Interface*, **est une interface qui permet aux logiciels de communiquer entre eux sur un réseau ou sur un même appareil.** Le plus souvent les développeurs utilisent des API REST pour créer des services web. Souvent appelés services web RESTful, REST utilise des méthodes HTTP (Post, get, put, delete) pour récupérer et publier des données entre un périphérique client et un serveur même s’ils utilisent des systèmes d’exploitation et des architectures différents. Le client peut demander des ressources avec un langage que le serveur comprend, et le serveur renvoie la ressource avec un langage que le client accepte. Le serveur renvoie la ressource au format JSON (JavaScript Object Notation), XML (Extensible Markup Language) ou texte, mais de nombreuses API prennent en charge d’autres langages. ![image](https://user-images.githubusercontent.com/75088424/123944859-d74a5d80-d99d-11eb-8a73-370c2d5a5811.png)|
| CRUD | **CRUD désigne les quatre opérations de base pour la persistance des données, en particulier le stockage d'informations en base de données.** **Create** (créer), **Read** ou Retrieve (lire), **Update** (mettre à jour), **Delete** ou Destroy (supprimer) En fonction de l’environnement de langage informatique, les opérations CRUD sont exécutées différemment, comme indiqué ci-dessous dans le tableau: ![image](https://user-images.githubusercontent.com/75088424/123945986-031a1300-d99f-11eb-801f-8eb44dff9fe1.png)|
| ORM | object-relational mapping (= mapping / cartographie objet-relationnel) est **un type de programme informatique qui se place en interface entre un programme applicatif et une base de données relationnelle pour simuler une base de données orientée objet.** On pourrait le désigner par là, « comme une couche d'abstraction entre le monde objet et monde relationnel ». Ce programme définit des correspondances entre les schémas de la base de données et les classes du programme applicatif.  Du fait de sa fonction, on retrouve ce type de programme dans un grand nombre de frameworks sous la forme de composant ORM qui a été soit développé, soit intégré depuis une solution externe. Ex: Sequelize |

### BASE DE DONNÉES

| Terme technique  | Définition & différence si besoin |
| - | - |
| Clés  | L'ensemble constitué d'une **clé primaire** et d'une **clé étrangère** sert à établir des relations entre tables.  |
| Clés **primaires** |  Une clé primaire est **le champs qui permet d'identifier de manière unique un enregistrement dans une table.** Souvent elle se nomme "id" et c’est un champ SERIAL (un entier auto incrémenté par la bdd). |
| Clés **étrangères** |les clés étrangères, dans une base de données relationnelle, **permettent de gérer des relations entre plusieurs tables et garantissent l'intégrité référentielle entre deux tables.** Une clé étrangère de ma table A' se réfère à la clé primaire de la table A. Seule une clé primaire peut être référencée par une clé étrangère. Ainsi, les clés étrangères ont pour fonction la vérification de l'intégrité de la base. |
| SGBD | Un *Système de Gestion de Base de Données* est **un logiciel qui permet de stocker des informations dans une base de données. Il permet de lire, écrire, modifier, trier, transformer ou même imprimer les données qui sont contenus dans la base de données.** Parmi les logiciels : systèmes libres (MySQL, PostgreSQL...), systèmes propriétaires (Oracle Database, Microsoft SQL Server...), embarqués ( SQLite...), NoSQL (Cassandra, Redis, MongoDB...), autres ( Access, OpenOffice.org Base, Neo4j...) |
| SGBDR | Un *Système de Gestion de Base de Données Relationnelle* est un logiciel standard qui repose sur les principes du modèle relationnel. Un SGBDR propose les trois principales fonctions suivantes : la définition des données sous forme de relations ; la manipulation des données par un langage déclaratif ; l’administration des données.  |
| MCD | *modèle conceptuel de données*, c'est **une représentation logique de l'organisation des informations et de leurs relations.** (méthode Merise). But: identifier les différentes entités et leurs relations ![image](https://user-images.githubusercontent.com/75088424/123967158-577cbd00-d9b6-11eb-9905-1737c8ba10aa.png) |
| MLD | *modèle logique (relationnel) de données*, la **traduction sous forme de relations du MCD.** But: identifier les différentes entités et leurs relations ![image](https://user-images.githubusercontent.com/75088424/123970321-500ae300-d9b9-11eb-8e2e-60c99f842e04.png)|
| MPD | *modèle Physique de données*, est la traduction du MLD dans le SGBDR choisi en tenant compte des contraintes de ce dernier. Deux représentations: SQL (create table) ou graphique(tableau...). Il n'y a pas de représentation spécifique |
| create table | La commande CREATE TABLE permet de créer une table en SQL. La création d’une table sert à définir les colonnes et le type de données qui seront contenus dans chacun des colonne (entier, chaîne de caractères, date, valeur binaire …). ![image](https://user-images.githubusercontent.com/75088424/123970135-28b41600-d9b9-11eb-8906-60d06afe990b.png)|

### BONNES PRATIQUES

| Terme technique  | Définition & différence si besoin |
| - | - |
| Gestion de version | La gestion de versions consiste à **gérer l'ensemble des versions d'un ou plusieurs fichiers.**  Elle est appuiée par un outil (logiciel) permettant d’enregistrer, de suivre et de gérer plusieurs versions d’un fichier ou d’un code source. Il permet d’établir un historique de toutes les modifications effectuées sur un élément, pour ainsi avoir la possibilité de récupérer une version antérieure selon la date et l’heure de la sauvegarde, et ce en cas d’erreur ou de problème sur une version actuelle. Il permet aussi un meilleur travail collaboratif. ex: dépots Git (hébergés sur gitHub) |
| Test | Un test c'est **du code qui exécute du code afin de vérifier si le résultat obtenu est bien celui attendu.** Ca sert à vérifier que le code fonctionne comme attendu pour tous les cas, découvrir les bugs le plus tôt possible, stabiliser, empêcher les régressions, faire évoluer et améliorer le code, améliorer le code petit à petit (voit un bug, écrit un test reproduit le bug, corrige le bug, ajoute nu test pour s'assurer que le bug ne revient pas) |
| Test unitaire | **On teste une unité de code, une partie précise du code** (une fonction, un composant). Le principe est de tester pendant que l'on code ou dès que le fragment de code est fonctionnel. L'idée étant de limiter les régressions. On utilise un test runner (Mocha...) et un utilitaire pour les assertions (Chai...) |
| Test d'intégration | **On test l'assemblage de plusieurs parties de code**, par exemple back-end + front-end |
| Test système / fonctionnel | **on teste la conformité du système.** Ex: test UI / IHM (intéraction homme machine), test de performance / benchmarck, test de charge... |
| Test d'acceptation | **On teste le projet avec le client** pour s'assurer que tout soit conforme aux attentes / exigences |
| TDD | Test driven dévelopment (= développement piloté par les tests), **les tests sont écrits avant le code et le code devra s'y confronter.** Avantages: à l'instant on sait que le code fonctionne, pas de code non testé dans l'application finie, on écrit uniquement le code dont on a besoin pour la fonctionnalité en cours, on définit les contours de l'application à l'avance en écrivant le test, maintenance facilitée car pas de code inutile. Inconvénients: impression de perte de temps, processus de développement peut paraitre pénible, spécifications pas toujours assez claires pour écrire le test avant.|

### CONNAISSANCES DE BASE

| Terme technique  | Définition & différence si besoin |
| - | - |
| Front-end | les Mickey qui pensent qu'ils sont mieux que les autres |
| Back-end | les Mickey qui pensent qu'ils sont mieux que les autres |
| Back-office |  |
| IDE | |
| CMS vs Frameworks vs Libraries | |
| Dépendance |  |
| Token |  |
| Types de données |  |
| Client vs Serveur |  |
| Absolu vs relatif |  |
| Callback |  |
| JSON |  |
| Fonction vs Méthode |  |
| Variable vs Propriété |  |
| Variable vs Constante |  |
| Handler |  |
| Abstraction |  |
| Scope / Portée |  |
| Itération |  |
| Affectation |  |

### FRONT

| Terme technique  | Définition & différence si besoin |
| - | - |
| Interface utilisateur web **dynamique** vs **statique** | |
| Préprocesseur |  |
| Accessibilité |  |
| DOM |  |
| Media Queries |  |
| Responsive |  |
| Évènement |  |

### MÉTHODOLOGIE

| Terme technique  | Définition & différence si besoin |
| - | - |
| SCRUM | |

### POO 

| Terme technique  | Définition & différence si besoin |
| - | - |
| POO |  |
| Classe |  |
| Héritage |  |

### REQUÊTE 

| Terme technique  | Définition & différence si besoin |
| - | - |
| XHR |  |
| Requête HTTP  | |
| Paramètres vs Arguments  |  |
| Paramètres d'URL |  |
| GET vs POST |  |
| Corps de la requête |  |
| Headers |  |
| AJAX |  |

### SÉCURITÉ 

| Terme technique  | Définition & différence si besoin |
| - | - |
| OWASP | |

### SEO 

| Terme technique  | Définition & différence si besoin |
| - | - |
| Référencement **organique** vs **payant** | |

### SYSTÈME & MISE EN LIGNE

| Terme technique  | Définition & différence si besoin |
| - | - |
| Server : **machine** vs **logiciel** |  |
| Déploiement |  |
| LAMP/WAMP/MAMP |  |
| Recette |  |
| Préproduction |  |
