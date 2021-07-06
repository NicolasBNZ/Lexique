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
| Clés  | L'ensemble constitué d'une **clé primaire** et d'une **clé étrangère** sert à **établir des relations entre tables.**  |
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
| Front-end | ~~Les Mickey qui pensent qu'ils sont mieux que les autres~~ Le Front-end désigne **les éléments d’un site que l’on voit à l’écran et avec lesquels on peut interagir depuis un navigateur.** il s'agit des éléments composés de HTML, CSS et de Javascript, contrôlés par le navigateur web de l'utilisateur. |
| Back-end | ~~Les Mickey qui pensent qu'ils sont mieux que les autres~~ Le back end désigne **ce qui n'est accessible que par les administrateurs et les utilisateurs ayant des droits spécifiques et qui permet de gérer les contenus et les paramètres de votre site. Ce domaine comprends la gestion des bases de données, la logique de l’application, les API etc…** |
| Back-office | Appliqué aux sites web dynamiques (bien souvent un CMS), le terme back office désigne **l’interface permettant de gérer le contenu du site.** Le back-office est la coulisse où travaillent les administrateurs de site web, les webmasters. |
| Front-end Vs back end | ![image](https://user-images.githubusercontent.com/75088424/124092517-3d46eb80-da57-11eb-978d-c94e1fd8ec7d.png) |
| IDE |Integrated Development Environment (=environnement de développement intégré) est une **logiciel de création d'applications sur mesure pour les développeurs regroupant un environnement de programmation complet**. Un IDE se compose généralement d'un éditeur de code, d'un compilateur, d'un débogueur et d'un générateur d'interface graphique. Ex: Visual Studio, Aclipse, Aptana... |
| Module | Un module désigne **un fichier de code de programmation ou un fichier de bibliothèque statique ou dynamique. Il sert à bien marquer la séparation entre les fonctionnalités, entre les portions de code. Il faut ensuite l'importer / exporter** Pour reprendre l'image de la programmation objet, un module est **une instance unique qui n'utilise pas d'héritage et ne contient aucun module fils.** Chaque module peut exporter ou importer certains symboles comme des variables, des fonctions ou des classes. |
| Package | Regroupement de modules éventuellement hierarchique |
| Frameworks | Cadre de travail. Ensemble de classes et de fonctions (dans des modules?) qu'on a à disposition pour permettre d'avancer plus vite dans les développements (évite de les code nous même). Ex: Express.js, Angular, Aurelia, meteor |
| Library - Bibliothèque | Ensemble de classes et de fonctions (dans des modules?) qu'on a à disposition pour permettre d'avancer plus vite dans les développements (évite de les code nous même). Ex: React, Moments.js, jQuery |
| Frameworks vs Library | **Qui utilise/ controle qui?** **La Library: c'est notre code qui appelle / utilise la library. Ex: Dans le dév de mon app, à un moment, pour gérer les dates, j'appelle des fonctions de la Library moment.js. Ex: Dans react, j'appelle Router (à vérifier). Le framework, il appelle / utilise notre code quand il juge que c'est le moment. Il structure notre appli et impose son architecture. "le framework est l'application" Par ex: express.js met tout en place pour écouter les requêtes HTTP et y répondre quand on écrit (req, res) (à vérifier)  |
| CMS | *content Management System* ou *système de gestion de contenu* (SGC), c’est un **logiciel destiné à concevoir et à mettre à jour de manière dynamique des sites Web ou des applications multimédias sans avoir besoin de toucher au code source.** Il s’agit d’une couche intermédiaire entre la base de données et l’interface utilisateur. Les non techs peuvent nourrir le site. Ex: wordpress, drupal, wix... |
| Dependencies | **Packages dont votre projet a besoin pour pouvoir travailler en production.** Les packages sont installés et/ou téléchargés (npm ou yarn) depuis la liste dans package.json: ![image](https://user-images.githubusercontent.com/75088424/124470046-6212ca00-dd9b-11eb-8492-7ed3d6361e75.png) |
| DevDependencies  | **Packages qui ne sont nécessaires que pour le développement et les tests locaux. (et pas en production)** comme des programmes ou codes utilisés pour compiler, transpiler etc... |
| Token | Jeton, désigne un **"identificateur, un dispositif matériel ou logiciel nécessaire à un utilisateur pour accéder à une application ou à un système réseau de manière plus sécurisée.**  La **tokenisation** est le procédé permettant de remplacer une donnée critique par un élément équivalent qui n’aura aucune valeur intrinsèque ou signification exploitable une fois sortie du système. Un token doit être irréversible et généré de manière aléatoire.![image](https://user-images.githubusercontent.com/75088424/124481045-2a5e4f00-dda8-11eb-88d5-8c90882721a9.png) |
| Types de données | Nous distinguerons les 5 types suivants en JS : **booléen** : true, false - **numérique** : entier : -10, 12, 42, ...  flottant : 3.14, 42.0, -12.5, ... - **chaîne de caractères** : "Hello world!", 'Bonjour le monde!' - **tableau** : ['42', 42, 3.14, ...] - **objet** : {module: 'M2206', nom: 'Intégration web', semestre: 2, UE: 2, coefficient: 2} |
| Client vs Serveur |  **Un internaute connecté au réseau via son ordinateur et un navigateur Web est le client, le serveur est constitué par le ou les ordinateurs contenant les applications qui fournissent les pages demandées.** La consultation de pages sur un site Web fonctionne sur une architecture client–serveur. C'est le protocole de communication HTTP (ou XML socket) qui est utilisé. ![image](https://user-images.githubusercontent.com/75088424/124482653-cb99d500-dda9-11eb-9756-95033f410252.png)|
| Chemin d'accès absolu (langage côté serveur) | Il **se rapporte toujours au dossier parent du serveur (=racine).** On le reconnait par le fait que ce chemin d’accès commence toujours par un slash. Exemple : /dossier/page.php |
| Chemin d'accès relatif (langage côté serveur) | **La cible va être cherchée à partir du fichier exécuté.**  Exemple: dossier/page.php ou ./dossier/page.php ou ../dossier/page.php |
| Callback | Une callback est **une fonction placée comme argument dans une fonction.** La fonction de callback n’est exécutée que si elle est appelée par la fonction qui la contient. D’où le terme fonction de callback. ![image](https://user-images.githubusercontent.com/75088424/124490625-9f368680-ddb2-11eb-8f8a-c5887f83a586.png) ![image](https://user-images.githubusercontent.com/75088424/124490647-a65d9480-ddb2-11eb-824f-9584e1c1bb07.png)|
| Callback hell | Plusieurs fonctions peuvent être créées indépendamment et utilisées comme fonctions de callback. Celles-ci créent des fonctions à plusieurs niveaux. **Lorsque cet arbre de fonctions créé devient trop volumineux, le code devient parfois incompréhensible et n’est pas facile à factoriser.** Ceci est connu sous le nom de callback hell. En raison de ce problème, des promesses ont été introduites pour simplifier les activités différées. ![image](https://user-images.githubusercontent.com/75088424/124490855-e1f85e80-ddb2-11eb-88a8-1e5768c1b755.png) |
| JSON | *JavaScript Object Notation – Notation Objet issue de JavaScript* est **un format standard utilisé pour représenter des données structurées. En général il se base sur une structure d'objet JavaScript (couples nom/valeur)** (plus rarement sous forme de tableau) **Il est habituellement utilisé pour transmettre des données sur des sites web.** Exemple, envoyer des données depuis un serveur vers un client afin de les afficher sur une page web ou vice versa. C'est un format léger sous forme de chaines de caractères. Il est facile à lire ou à écrire pour des humains. Il est aisément analysable ou générable par des machines. https://developer.mozilla.org/fr/docs/Learn/JavaScript/Objects/JSON |
| Fonction vs Méthode | **Une methode est une fonction dans un objet.** les fonctions sont définies en dehors des classes, tandis que les méthodes sont définies à l'intérieur des classes et font partie de celles-ci. |
| Variable vs Propriété |  |
| Variable vs Constante | **Une constante *const* est similaire à une variable *var* au sens où c’est également un conteneur pour une valeur.** Cependant, à la différence des variables, on ne va **pas pouvoir modifier la valeur d’une constante.** En effet, une fois qu’une valeur est attribuée à une constante, celle-ci est attribuée de façon définitive et ne va pas pouvoir être modifiée. C’est d’ailleurs de là que les constantes portent leur nom : car leur valeur est constante. Les constantes vont être très utiles dans le cadre d’un script qui va réutiliser souvent la même valeur mais qui doit toujours utiliser cette valeur exactement. Dans ce cas-là, **plutôt que de réécrire la valeur à chaque fois, nous allons stocker la valeur dans une constante et utiliser la constante.** Dans ce cas-là, utiliser une constante va rendre notre script plus clair car on pourra rapidement identifier la valeur utilisée et également plus facilement maintenable car dans le cas où l’on doive modifier le script et cette valeur en particulier un jour, on n’aura alors qu’à modifier la constante plutôt que de modifier toutes les occurrences de la valeur dans le script. **Les constantes font partie de la portée du bloc (comme les variables définies avec let).** **La portée d'une variable déclarée avec var est le contexte d'exécution courant, c'est-à-dire : la fonction qui contient la déclaration ou le contexte global si la variable est déclarée en dehors de toute fonction.** |
| Handler | "gestionnaire", Il s'agit d'un terme très générique. **Une fonction / methode qui est déclenchée par un événement spécifique,** comme un message entrant, une exception levée, un signal envoyé à un processus, une demande d'entrée/sortie réseau ou un clic de souris sur un élément de l'interface utilisateur. ex: element.addEventListener('type_d_event', *fonctionHandler* ); |
| Abstraction | **Un mécanisme / une pratique servant à réduire le code d'un niveau de détail en proposant une représentation simplifiée.** https://onvaessayer.org/mobileCSP/unit2/2_08.php |
| Abstraction de données | Permet d'écrire des programmes plus généraux, facile à lier et à vérifier. Puis de **gérer des informations compliquées en masquant la complexité derrière un nom de variable.** Ex: une variable pokemon avec à l'intérieur le nom, les attaques... **On utilise la variable et pas les infos en littéral** |
| Abstraction procédurale | Permet de masquer les détails inutiles, de **regrouper à un seul endroit les tâches répétitives,** de rendre le code plus facile à lire, tester et faire évoluer. Ex: une fonction qui calcule un racine carré qu'on encapsule dans un composant et on appelle que la fonction de calcul. Le détail de l'opération est caché, on l'appelle quand on en a besoin et on ne la modifie qu'à un seul endroit  |
| Scope / Portée | **Le scope d’un objet est la portion de code dans laquelle une variable peut exister et maintenir une valeur qui lui aura été préalablement affectée.** En effet, en fonction de l'emplacement où vous déclarez votre variable et du type de variable (var, let, const), la portée de votre scope javascript peut être différente. https://cdiese.fr/le-scope-des-variables-en-javascript/#javascript_scope-var_let_const |
| Let et const | *const* et *let* permettent de déclarer une variable dans le scope d’un bloc de code. *let* autorise des affectations d’une nouvelle valeur à une variable. *const* interdit de nouvelles affectations. |
| Itération | (= **répétition d'un précessus**) **Procédé de calcul répétitif qui boucle jusqu'à ce qu'une condition particulière soit remplie.** Répétition d'un calcul, d'une opération, d'un raisonnement. Le processus d'itération est employé fréquemment en algorithmique. Ex: **boucle for... of**, "à chaque itération". |
| Affectation | On appelle affectation le fait de donner une certaine valeur à une variable. **Affecter une valeur à une variable** signifie écrire cette valeur dans la case mémoire représentée par la variable. Pour réaliser une affectation en JavaScript on utilise le signe =. Ex var chemise = 4 |

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
| backlog  |Le backlog est **une liste de tâches priorisées définissant les caractéristiques d’un produit.** Il est un des éléments fondamentaux de la méthodologie Scrum. Il s’agit de l’outil de travail principal du Product Owner qui se charge de recueillir les besoins auprès des parties prenantes et de les transformer en liste de fonctionnalités prêtes à être développées par l’équipe de développement. Communément **on peut formaliser ce items sous forme de *Users Stories* ** |

### POO 

| Terme technique  | Définition & différence si besoin |
| - | - |
| POO |  |
| Classe | (à affiner) Une classe définit toutes les propriétés qui caractérisent un certain ensemble d'objets. Une classe est abstraite par opposition à un membre particulier d'un ensemble d'objets qu'elle décrit. Par exemple, la classe Employee pourrait représenter l'ensemble de tous les employés. |
| instance | (à affiner) Le terme instance a une signification technique spécifique dans les langages basés sur les classes. Dans ces langages, une instance est une instanciation individuelle d'une classe et est fondamentalement différente d'une classe. En JavaScript, « instance » n'a pas cette signification technique car **JavaScript ne fait pas cette différence entre classes et instances. Toutefois, en parlant de JavaScript, le terme « instance » peut être utilisé de manière informelle pour désigner un objet créé à l'aide d'une fonction de construction particulière.** De façon informelle on peut dire: La class c’est un moule pour le gâteau, l’instance c’est quand je fais un gâteau |
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
