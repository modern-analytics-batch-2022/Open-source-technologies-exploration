## Dagster
![dagster-logo](https://user-images.githubusercontent.com/98336381/154458771-6e67f173-bd0c-4e28-8f0d-efb579a4c794.png)

### Brief description of Dagster technology
Une plateforme d'orchestration pour le développement, la production et l'observation des actifs de données.
Dagster vous permet de définir des tâches en termes de flux de données entre des composants logiques réutilisables, puis de les tester localement et de les exécuter partout. Grâce à une vue unifiée des tâches et des ressources qu'elles produisent, Dagster peut programmer et orchestrer Pandas, Spark, SQL ou tout autre élément que Python peut invoquer.

### General information
* Creation year : 2018 

* Website       : https://dagster.io

* Github repo  : https://github.com/dagster-io/dagster

* Communiy size  : bien que la technologie Dagster est encore nouvelle mais son communauté s'agrandit.

* Founders  :  Nick Schrock Founder of *Elementl* ![nick](https://user-images.githubusercontent.com/98336381/154588598-99ae826b-bc2e-490d-b151-c996e3dba038.jpg)


### Main capabilities  
* Dagster permet de développez et testez localement, puis déployez n'importe où. 
* modéliser et saisir les données produites et consommées par chaque étape.
* Lier les données aux calculs.
* Créer une plateforme de données en libre-service.
* Permet d'éviter les problèmes des dipendances.
* Déboguer les pipelines à partir d'une interface utilisateur trés riche.

### Available connectors / integrations  

Dagster dispose de nombreuses librairies d'intégration dont les principales sont :
* Airbyte : dagster-airbyte
* Flux d' air : dagster-airflow
* AWS : dagster-aws
* Azure : dagster-azur
* Céleri : dagster-céleri
* Céleri + Docker : dagster-céleri-docker
* Céleri + Kubernetes : dagster-celery-k8s
* Dask : dagster-dask
* Databricks : dagster-databricks
* Datadog : dagster-datadog
* Docker : dagster-docker
* dbt : dagster-dbt
* Fivetran : dagster-fivetran
* GCP : dagster-gcp
* GraphQL : dagster-graphql
* De grandes attentes : dagster-ge
* Github : dagster-github
* Kubernetes : dagster-k8s
* Microsoft Teams : dagster-msteams
* MLflow : dagster-mlflow
* MySQL : dagster-mysql
* PagerDuty : dagster-pagerduty
* Pandas : dagster-pandas
* Moulin à papier : dagstermill
* Papertrail : dagster-papertrail
* PostgreSQL : dagster-postgres
* Prométhée : dagster-prometheus
* Pyspark : dagster-pyspark
* Shell: coquille de poignard
* Slack : dagster-slack
* Flocon de neige: dagster-flocon de neige
* Étincelle : dagster-étincelle
* SSH/SFTP : dagster-ssh
* Twilio : dagster-twilio



### deployment:
Dagster peut être installé et configuré pour s'exécuter de différentes manières dans différents environnements :
Ses différents exécuteurs sont responsables de l'exécution des étapes d'une exécution de travail. Une fois l'exécution démarrée et le processus d'exécution, ou la tâche d'exécution, alloué et démarré, l'exécuteur assume la responsabilité de l'exécution. Les exécuteurs peuvent aller des exécuteurs en série à processus unique à la gestion des ressources informatiques par étapes avec un plan de contrôle sophistiqué.
* in_process_executor: Le plan d'exécution s'exécute en série sur l'opérateur d'exécution lui-même.
* multiprocess_executor: Chaque étape s'exécute dans son propre processus généré. Il a un niveau configurable de parallélisme.
* dask_executor: exécute chaque étape d'une tâche.
* celery_executor: Exécute chaque étape dans le céleri de la tâche.
* docker_executor: exécute chaque étape dans un conteneur Docker.
* k8s_job_executor : exécute chaque étape dans des pods Kubernetes éphémères.
* celery_k8s_job_executor : exécute chaque étape dans un pod Kubernetes éphémère, en utilisant le céleri comme plan de contrôle pour la hiérarchisation et la mise en file d'attente.
* celery_docker_executor: exécute chaque étape dans un conteneur Docker, en utilisant le céleri comme plan de contrôle pour la hiérarchisation et la mise en file d'attente.

Dagster peut être installé et utilisé en cloud dans différents environnements, tels que :

* Responsable de la communication Kubernetes
* Dagster en tant que service
* Docker
* AWS
* GCP
* Exécuté via Céleri
* Exécuté via Dask


### Reviews
__Good reviews__ :
* Flexibilité : Les utilisateurs disposent de nombreux degrés de liberté pour configurer l'allocation des ressources de calcul.
* Évolutivité horizontale : chaque processus de calcul spécifique à une exécution s'exécute indépendamment. Fonctionne à l'échelle horizontale.
* Cloud-Native : les ressources de calcul éphémères tirent parti du calcul entièrement élastique dans les clouds publics.


__Bad reviews__ :
* Dagster n'est pas facile a utiliser.



### Roadmap  

![roadmap](https://user-images.githubusercontent.com/98336381/154602021-072843fb-d04a-4f7f-a4ff-f50221ddb5e2.png)

### References 
* Dagsteer Documentation.
* Dagster blog & Dagster repository on github.
* these : *A Survey of Big Data Pipeline Orchestration Tools from the Perspective of the DataCloud Project* Link : http://ceur-ws.org/Vol-3036/paper05.pdf
