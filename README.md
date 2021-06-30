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
| Clés **primaires** vs Clés **étrangères** | |
| SGBD | |

### BONNES PRATIQUES

| Terme technique  | Définition & différence si besoin |
| - | - |
| Gestion de version |  |
| Tests automatisés |  |

### CONNAISSANCES DE BASE

| Terme technique  | Définition & différence si besoin |
| - | - |
| Front-end vs Back-end| |
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
