<html>
<h1 align="center">E-Banking Application</h1>
<br>
<p>Cette application web a été créée pour faciliter la gestion de vos comptes bancaires. Elle repose sur la technologie Spring Boot pour le développement du backend et Angular pour le frontend.</p>
<h2>Description</h2>
<p>L'Application Bancaire Numérique propose une gamme de fonctionnalités permettant de gérer divers types de comptes bancaires. Parmi ces types de comptes, on retrouve le Compte Courant et le Compte Épargne. Chaque compte est doté d'un identifiant unique et possède des caractéristiques spécifiques en fonction de son type. Les Comptes Courants sont associés à un attribut de découvert autorisé, tandis que les Comptes Épargne bénéficient d'un taux d'intérêt.</p>
<p>En plus des informations spécifiques à chaque compte, tels que son type et ses attributs, chaque compte bancaire conserve un historique détaillé des opérations effectuées. Chaque opération est identifiée par un identifiant unique et comprend également une date, un montant, une description et un type (débit, crédit ou transfert). L'historique du compte enregistre également le solde du compte après chaque opération, fournissant ainsi une trace complète de toutes les transactions effectuées.</p>
<p>
Les clients sont enregistrés dans le système avec les attributs suivants : identifiant, nom et adresse e-mail. Chaque client a la possibilité d'avoir plusieurs comptes bancaires associés à son profil, leur permettant ainsi de gérer plusieurs comptes simultanément.</p>
<h2>Backend</h2>
<p>Le backend de l'Application Bancaire Numérique est développé en utilisant Spring Boot. Il offre des API RESTful pour effectuer différentes opérations sur les comptes bancaires et les clients. L'architecture du backend suit une approche en couches et comprend les éléments suivants :</p>
<h3>Contrôleurs</h3>
<p>Les contrôleurs assurent la gestion des requêtes entrantes en les acheminant vers les services appropriés pour leur traitement. Leur responsabilité principale consiste à associer les points d'accès de l'API aux actions correspondantes, tout en vérifiant la validité des paramètres de requête.</p>
<h3>Services</h3>
<p>Les services regroupent la logique métier essentielle de l'application, prenant en charge des fonctionnalités clés telles que la création de comptes bancaires, l'exécution des opérations, l'accès aux détails du compte et la gestion des informations clients. Ils sont chargés de garantir le bon fonctionnement des processus centraux de l'application.</p>
<h3>Repositories</h3>
<p>Les repositories sont responsables de l'interaction avec la base de données pour effectuer des opérations CRUD (Create, Read, Update, Delete). Ils offrent une couche d'abstraction entre l'application et le stockage des données sous-jacent, permettant ainsi de manipuler les données de manière efficace et cohérente. En utilisant les repositories, l'application peut interagir avec la base de données de manière indépendante, sans se soucier des détails spécifiques de la mise en œuvre du stockage des données.</p>
<h3>Entités</h3>
<p>Les entités sont les représentations des objets métier au sein de l'application. Elles sont mappées sur des tables de base de données et définissent la structure des données. Les entités encapsulent les attributs et les comportements des objets métier, et elles sont utilisées pour manipuler et persister les données de manière cohérente. En reliant les entités aux tables de base de données, on assure la synchronisation entre la logique métier de l'application et la persistance des données.</p>
<h3>Objets de Transfert de Données (DTO)</h3>
<p>Les DTO (Data Transfer Objects) sont employés pour faciliter le transfert de données entre le backend et le frontend. Ils regroupent les informations pertinentes et offrent une représentation structurée des données. Les DTO servent de conteneurs pour les données échangées, permettant une communication efficace entre les différentes parties de l'application. En encapsulant les données nécessaires, ils contribuent à garantir une transmission claire et cohérente des informations entre le backend et le frontend.</p>
<h2>Frontend</h2>
<p>
Le frontend de l'Application Bancaire Numérique est développé en utilisant Angular, qui fournit une interface conviviale pour interagir avec l'application.</p>
<p>L'architecture du frontend est basée sur une approche composant. Elle comprend les éléments suivants:</p>
<h3>Composants</h3>
<p>
Les composants sont chargés du rendu de l'interface utilisateur et de la gestion des interactions de l'utilisateur. Ils encapsulent des fonctionnalités spécifiques et peuvent être réutilisés sur différentes pages. Les composants jouent un rôle clé dans la création d'une interface utilisateur modulaire et maintenable, en divisant les fonctionnalités en unités indépendantes et réutilisables. Ils permettent également une séparation claire entre la logique de présentation et la logique métier, favorisant ainsi une gestion plus efficace du code et une évolutivité de l'application.</p>
<h3>Services</h3>
<p>Les services du frontend sont responsables de la communication avec les API du backend. Ils se chargent des requêtes HTTP pour récupérer les données nécessaires et mettent ensuite à jour l'interface utilisateur en conséquence. En résumé, les services du frontend assurent la liaison entre l'application frontend et les fonctionnalités fournies par le backend, en gérant la récupération et la manipulation des données nécessaires pour offrir une expérience utilisateur fluide et réactive.</p>
<h3>Modèles</h3>
<p>Les modèles dans le frontend sont des représentations structurées des données utilisées dans l'application. Ils correspondent aux DTO (Data Transfer Objects) du backend et assurent une cohérence dans le format des données. En résumé, les modèles dans le frontend permettent de définir la structure des données nécessaires à l'application, en reflétant les DTO du backend et en garantissant une manipulation homogène des données tout au long du processus de développement.</p>
<h2>Premiers pas</h2>
<p>Pour exécuter l'Application Bancaire Numérique en local, suivez ces étapes :</p>
<ol>
  <li>Clonez le dépôt depuis "https://github.com/MarouaneBcht/Digital-Banking.git".</li>
  <li>Configurez le backend en mettant à jour les fichiers de configuration nécessaires, tels que les paramètres de la base de données et les points d'accès de l'API.</li>
  <li>Compilez et exécutez l'application backend à l'aide de votre IDE préféré ou en exécutant les commandes Maven appropriées.</li>
  <li>Configurez le frontend en mettant à jour les URL des points d'accès de l'API pour correspondre à votre configuration backend.</li>
  <li>Installez les dépendances requises pour le frontend en utilisant `npm install`.</li>
  <li>Compilez et exécutez l'application frontend en utilisant `ng serve`.</li>
  <li>Accédez à l'application dans votre navigateur à l'adresse `http://localhost:4200`.</li>
</ol>
<h2>Conclusion</h2>
<p>L'Application Bancaire Numérique offre une solution complète pour la gestion des comptes bancaires et l'exécution d'opérations bancaires. Grâce à son backend basé sur Spring Boot et son frontend basé sur Angular, elle propose une interface robuste et conviviale à la fois pour les clients et les administrateurs bancaires. L'application prend en charge diverses fonctionnalités telles que la création de profils clients, l'ouverture de différents types de comptes bancaires, l'exécution de transactions de débit et de crédit, le transfert de fonds entre les comptes et la consultation de l'historique des transactions.</p>
<p>En utilisant la puissance de Spring Boot et d'Angular, l'application garantit l'évolutivité, la sécurité et une expérience utilisateur transparente. Son architecture modulaire permet une extension et une personnalisation faciles, ce qui la rend adaptée aux améliorations futures et à l'intégration avec d'autres systèmes.</p>
<p>Pour commencer avec l'Application Bancaire Numérique, il vous suffit de suivre les instructions fournies dans la section "Premiers pas" ci-dessus. N'hésitez pas à explorer les dépôts backend et frontend pour comprendre les détails de mise en œuvre et contribuer au projet.</p>