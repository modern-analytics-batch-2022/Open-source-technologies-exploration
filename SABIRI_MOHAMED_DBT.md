#### DBT : DATA TRANSFORMATION
![DBT1](https://user-images.githubusercontent.com/97849043/154369096-22a739ce-c052-4472-a9c6-b4308daf3e9d.jpg)

### INTRODUCTION 

De nos jour la recherche et l’exploitation des outils d’analyse des base données NoSQL ou Big Data constitue un point très importante pour les analystes dans le processus ETL ou ELT (Extraction, Transformation, Chargement de données), alors que dans chaque un de ces opération nous somme dans l’obligation d’intégration des outils pour garder la fiabilité des résultats ainsi que la rapidité de traitement de données. Dans ce sujet je vais aborder l’outils BDT (Data Build Tool) outils utilisé dans l’étape de transformation des données dans les entrepôts de données.

### DEFINITIONS 

•	Data Build Tool
DBT outils permettant les Analytics et les ingénieurs d'analyse de faire la transformation les données dans leurs entrepôts en écrivant simplement des instructions de sélection. il gère la transformation de ces instructions select en tables et vues, aussi effectue les processus T dans ELT(Extract, Load, Transform) par contre il n'extrait ni ne charge de données, mais il est extrêmement efficace pour transformer des données déjà chargées dans les entrepôt

**### Brief description:**
## Historique :

•	**2016** : commencé chez RJMetrics

•	**2018** : acquis par Talend, avec lancement du 1ere produit commercial

•	**2020** : En avril 2020, dbt Labs a annoncé sa série A dirigée par Andreessen Horowitz, En novembre, dbt Labs a annoncé sa série B dirigée par Andreessen Horowitz et Sequoia.

•**2021** : dbt Labs a relevé sa série C dirigée par Altimeter, Sequoia et Andreessen Horowitz.

## Site Internet

•	https://docs.getdbt.com/

 **Dépôt GitHub** 

•	https://github.com/dbt-labs/

 **Taille de la communauté** 

•**Octobre 2018**: mise à jour du nombre d'utilisateurs dbt au début du post de 100 à 280

•**Septembre 2019**: mise à jour du nombre d'utilisateurs dbt au début de la publication de 280 à 850

•**Mai 2021**:nombre d'utilisateurs dbt mis à jour au début de la publication à 5000 

### FONDATEURS
  
![dbt2](https://user-images.githubusercontent.com/97849043/154371089-356abc07-2f15-4aef-a29f-53b9d7d6674a.png)

### FONCTIONNALITES PRINCIPALES  

 ![DBT3](https://user-images.githubusercontent.com/97849043/154371407-76fc6d3e-84c2-400e-aaf8-d3d8c8b5516c.png)

Dans le processus ETL le DBT est utilisé pour objectif de faire la transformation de données, et comme illustrer dans le workflow, on distingue les fonctionnalité suivantes qui sont déduite de trois couches constituant le model DBT :


**Develop : développer**

Écrivez des modèles SQL modulaires avec des instructions SELECT et la fonction ref() - dbt gère la corvée de gestion des dépendances.

**Test & Document : Tester et documenter**

Testez chaque modèle avant la production et partagez la documentation générée dynamiquement avec toutes les parties prenantes des données.

**Deploye : Contrôle de version et CI/CD**

Déployez en toute sécurité à l'aide d'environnements de développement. Le contrôle de version activé par Git permet la collaboration et un retour aux états précédents

### CONNECTIVITE ET INTEGRATION
  Comme objectif de BDT est de faire la transformation des données dans les bases de données, Entrepôt de données ou dans les plate-forme et clous, son fonctionnement dépond de la possibilité à intégrer avec le type de SGSB des données à transformer, alors que son utilisation fonctionne par utilisation des adaptateur de fonctionnement. 

![DBT4](https://user-images.githubusercontent.com/97849043/154371801-43fe2b2a-86b6-44c5-9988-a4e24425d043.PNG)

### DEPLOIEMENT
Architecture de déploiement réseau de DBT.

<img width="533" alt="DBT5" src="https://user-images.githubusercontent.com/97849043/154371908-b7e9f5ce-8246-4800-a30c-7dc0d3ac2970.png">

Selon le schéma précèdent on distingue les sections suivantes : 

•	VPC : Dans les deux déploiements hébergés, l'infrastructure d'application dbt Cloud réside dans un VPC. AWS géré par dbt Labs. L'une des principales différences entre le déploiement de production et le déploiement à locataire unique est que le déploiement à locataire unique fournit un VPC dédié pour un seul client.

•	EKS : Elastic Kubernetes Service permet de  gérer les ressources d'application dbt Cloud. EKS offre un degré élevé de fiabilité et d'évolutivité pour l'application dbt Cloud.

•	CLB : un ou plusieurs équilibreurs de charge classiques AWS vivant dans un sous-réseau public sont exploités dans les environnements de déploiement hébergés pour distribuer le trafic entrant sur plusieurs instances EC2 dans le cluster EKS.

•	EC2 : les déploiements dbt Cloud hébergés exploitent un cluster de nœuds de travail AWS EC2 pour exécuter l'application dbt Cloud.

•	EBS : Afin de stocker les données d'application, dbt Cloud exploite AWS Elastic Block Store monté sur les instances EC2 décrites ci-dessus.

•	EFS : Un système de fichiers élastique AWS est provisionné pour les déploiements hébergés afin de stocker et de gérer les fichiers locaux à partir de dbt Cloud IDE.
•	S3 : AWS Simple Storage Service (S3) est utilisé pour stocker les journaux d'application et les artefacts dbt Cloud (tels que ceux générés à partir des exécutions de tâches dbt).

•	RDS : L'application hébergée dbt Cloud exploite AWS Postgres RDS pour stocker les informations d'application telles que les comptes, les utilisateurs, les environnements, etc. Notez que, comme expliqué dans la section Interaction de l'entrepôt de données ci-dessus, aucune donnée d'un entrepôt associé n'est jamais stockée dans cette base de données.



### LES PRATIQUES

Les recommandations des bonnes pratiques DBT :

1.	Utiliser la fonction de références.
2.	Limiter les références aux données brutes
3.	Renommer et reformuler les champs une fois
4.	Décomposez des modèles complexes en plus petits morceaux
5.	Regroupez vos modèles dans des répertoires
6.	Ajoutez des tests à vos modèles
7.	Considérez l'architecture de l'information de votre entrepôt de données
8.	Utiliser la syntaxe de sélection de modèle lors d'une exécution locale
9.	Conseils professionnels pour les flux de travail
10.	N'exécutez que des modèles modifiés pour tester les modifications (« CI mince »)
11.	Limiter les données traitées en développement
12.	Utiliser des crochets pour gérer les privilèges sur les objets créés par dbt
13.	Séparez les transformations centrées sur la source et centrées sur l'entreprise
14.	Gestion des espaces blancs générés par Jinja

## Les principaux commande de DBT


•	build: build and test all selected resources (models, seeds, snapshots, tests)

•	clean (CLI only): deletes artifacts present in the dbt project

•	compile: compiles (but does not run) the models in a project

•	debug (CLI only): debugs dbt connections and projects

•	deps: downloads dependencies for a project

•	docs : generates documentation for a project

•	init (CLI only): initializes a new dbt project

•	list (CLI only): lists resources defined in a dbt project

•	parse (CLI only): parses a project and writes detailed timing info

•	run: runs the models in a project

•	seed: loads CSV files into the database

•	snapshot: executes "snapshot" jobs defined in a project

•	source: provides tools for working with source data (including validating that sources are "fresh")

•	test: executes tests defined in a project

•	rpc (CLI only): runs an RPC server that clients can submit queries to

•	run-operation: runs arbitrary maintenance SQL against the database


