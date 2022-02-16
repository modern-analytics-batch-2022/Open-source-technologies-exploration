## Apach Airflow
![airflow](https://user-images.githubusercontent.com/97967656/154340205-5a0fbe54-7b30-4b2b-9182-d702f1f262b8.png)

### Brief description 
Apache Airflow est une plateforme de planification de flux de travail open-source, très utilisée dans le domaine de l’ingénierie des données. Découvrez tout ce que vous devez savoir au sujet de cet outil du Data Engineer : 
fonctionnement, cas d’usage, composants principaux.
La plateforme Apache Airflow permet de créer, de planifier et de surveiller des workflows (flux de travail) par le biais de la programmation informatique. Il s’agit d’une solution totalement open source, très utile pour 
l’architecture et l’orchestration de pipelines de données complexes et le lancer de tâches.

![DAG](https://user-images.githubusercontent.com/97967656/154355806-23ee67a7-c3fc-433b-b774-cd6529fac576.JPG)
------------------------------

![user](https://user-images.githubusercontent.com/97967656/154358700-d8ed48b3-5ea0-485d-8791-14be75490b7d.JPG)


### General information
 * Année création : 2016
 * Site Web : airflow.apach.org
 
 * Dépôt Github : github.com/apach/airflow
 
 * Chaine communauté : https://apache-airflow-slack.herokuapp.com/
 
 * Taille communauté : 14 308 (08/02/2022)
 
 * Développer par : Apach Software fondation
 
 
### Main capabilities  
* Dynamique
* Extensible
* Elégant
* Evolutive.

### Available connectors 
* Amazon Web Services (AWS) :

![aws](https://user-images.githubusercontent.com/97967656/154358014-0439e68e-3aa0-4dc3-8938-af5859d4add3.JPG)

* Google Cloud Platform (GCP):

![gcp](https://user-images.githubusercontent.com/97967656/154358145-e99cc1a8-6d92-455d-a877-33d2776a9ade.JPG)

### integrations

* API Authentication backends
* Email backends
* Executor
* Kerberos
* Logging
* Metrics
* Operators and hooks
* Plugins
* Screts backends
* Tracking system

### Ways to deploy it :
## 1- DÉPLOYER AIRFLOW SUR AWS EKS
Kubernetes est la solution éprouvée pour la mise à l'échelle automatique, l'élasticité et la gestion automatique des ressources. 
Il existe une énorme communauté qui soutient les initiatives Kubernetes et, par conséquent, plusieurs fichiers de configuration prêts 
à l'emploi sont disponibles pour déployer Airflow à l'aide d'EKS. EKS continue de générer de nouveaux nœuds avec l'exécuteur ou le planificateur 
Airflow pour gérer les charges de travail nouvelles et lourdes.

### 2- DÉPLOYER AIRFLOW SUR AWS EC2

Le déploiement d'Airflow sur EC2 est presque identique à celui que vous déploieriez sur une machine virtuelle sur site : déploiement simple et agréable 
à l'ancienne, capacité préconfigurée, nœuds fixes dans le cluster et équilibrage de charge prédéterminé. Un ensemble d'instances EC2 dédiées prend en 
charge les composants du serveur Web et un autre ensemble d'instances EC2 héberge le planificateur et les exécuteurs.
Ce modèle de déploiement offre peu de dynamisme en termes de  scale-up ou scale-down et la disponibilité de la solution dépend du  nombre d'instances 
provisionnées en amont. Cela fonctionne bien dans un scénario où  les charges de travail sont assez fixes et la croissance est minimale ou constante.
Il ne peut pas du tout gérer les pics de charge.

### 3- UTILISER LE SERVICE MANAGED AIRFLOW SUR AWS

AWS fournit une variété d'options pour le déploiement d'Airflow qui peuvent être classées en IaaS, PaaS et SaaS.
Amazon Managed Workflows for Apache Airflow (MWAA) est un service d'orchestration géré dans son état naissant à partir de maintenant en 2021. 
Il s'agit d'une offre SaaS qui promet de répondre aux préoccupations les plus courantes concernant l'évolutivité, la disponibilité et la sécurité. 
Comme tout autre service, il est facile à démarrer, cependant, il n'a pas encore fait ses preuves dans l'industrie.
Il a le pouvoir de devenir l'un des  modèles de déploiement d'Airflow les plus recherchés car il est pré-intégré à d'autres  services éprouvés d'AWS,
tels qu'Amazon S3, CloudWatch, IAM et autres.


### Reviews
## Good reviews :

* Gestion des dépendances,
* Modèles et macros,
* Plusieurs opérateurs,
* Interfaces utilisateurs et journaux,
* Basé sur les principes fonctionnels,
* en source.

## Bad reviews :

* Le modèle de traitement de données, n’est pas intuitif pour les nouveaux ingénieurs,
* La modification de l’intervalle de planification, nécessite de renommer le DAG,
* Pas de support Windows natif.

### Roadmap  
La page feuille de route est temporairement masquée. Lorsque le contenu est prêt, rajoutez la page enmettant le code suivant dans l’avant propos:

  ........
  
    Title : "Roadmap"
    
    linkTitle : "Roadmap"
    
    showSideNav : false
    
    menu :
    
    weight:15
    
    .....
    
## Titre principale A
Le but du script est de définir un objet DAG. Il doit être évalué rapidement, car le planificateur l’exécute périodiquement pour refléter les modifications éventuelles.

## Titre principale B
Différentes tâches s’exécutent sur différents travailleurs à différents travailleurs à différents moments, ce qui signifie que ce script ne peut pas être utilisé par une
communication croisée entre les tâches.

## Avantage 

![cons](https://user-images.githubusercontent.com/97967656/154363952-69329af4-6060-441f-9fae-d2ad5bfd5022.JPG)

## Inconvénients 

![limit](https://user-images.githubusercontent.com/97967656/154364290-cd724275-c73f-4007-9cbb-db47c0bf898e.JPG)

## Conclusion
Malgré tous les inconvénients d'Apache Airflow, il fournit toujours un excellent cadre de traitement de données par lots pour gérer ETL. De nombreuses entreprises utilisent
Airflow pour les avantages qu'il offre.
