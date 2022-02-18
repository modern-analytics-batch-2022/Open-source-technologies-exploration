## Elasticsearch


### Brief description 

Elasticsearch est un moteur de recherche et d'analyse distribué gratuit et ouvert pour tout type de données, y compris les données textuelles, numériques, géospatiales, structurées et non structurées. Elasticsearch a été conçu à partir d'Apache Lucene. Réputé pour ses API REST simples, sa nature distribuée, sa vitesse et sa scalabilité, Elasticsearch est le composant principal de la Suite Elastic ELK (Elasticsearch, Logstash et Kibana) : Elasticsearch est associé à deux autres produits open source : le visualiseur de données Kibana et l'outil d'extraction, de transformation et de chargement de données (ETL) Logstash.

### General information

#### Creation year
Shay Banon a publié la première version d'Elasticsearch en février 2010
#### Website  
https://www.elastic.co/fr/elasticsearch/
#### Github repo  
https://github.com/elastic/elasticsearch
#### Community channel  
https://www.youtube.com/c/officialelasticcommunity
#### Communiy size  
Elastic compte plus de 150 groupes d'utilisateurs dans 52 pays du monde avec environ 80 000 + membres.
#### Founders    
Shay Banon, Steven Schuurman, Uri Boness, Simon Willnauer  
### Main capabilities  
Elasticsearch fournit un ensemble complet et puissant d'API REST pour effectuer des tâches comme la vérification de la santé du cluster, des opérations CRUD (création, lecture, mise à jour, suppression), rechercher des opérations à partir d'indices et exécuter des opérations de recherche avancées comme le filtrage et les agrégations.
•	Il est possible d'exploiter les fonctionnalités de recherche et d'analyse en temps réel d'Elasticsearch sur des données volumineuses en utilisant le connecteur Elasticsearch-Hadoop (ES-Hadoop).
•	Des outils comme Kibana et Logstash permettent de donner un sens aux données de manière très simple et immédiate en utilisant des graphiques et en effectuant des recherches granulaires.

### Available connectors / integrations  
Elasticsearch utilise des API RESTful et JSON standard. Il offre plusieurs connecteurs pour prendre en charge une multitude de langages de programmation:
* Java
* JavaScript (Node.js)
* Go
* .NET (C#)
* PHP
* Perl
* Python
* Ruby

### Ways to deploy it :
#### On-prem  
Elasticsearch peut être téléchargé et installé sur votre propre matériel ou dans le cloud. La documentation Elasticsearch donne des instructions pour télécharger, installer et configurer Elasticsearch.

#### PaaS / SaaS  
Elasticsearch peut être déployé en tant que service hébergé et géré à travers Elasticsearch Service, disponible sur Amazon Web Services (AWS), Google Cloud et Alibaba Cloud.
Pour les utilisations souhaitant provisionner, gérer et monitorer leurs déploiements depuis une seule console, mais préfèrent ne pas utiliser une plateforme de cloud public, Elastic propose Elastic Cloud Enterprise (qui peut être déployée sur des clouds privés et publics, des machines virtuelles ou du matériel de serveur physique).

### Reviews
#### Good reviews

* Elasticsearch est open source et gratuit
* Elasticsearch est rapide
* Elasticsearch est hautement distribué
* Elasticsearch est naturellement distribué
* Elasticsearch dispose d'une multitude de fonctionnalités
* La Suite Elastic (ELK Elasticsearch Logstash Kibana) simplifie l'ingestion, la visualisation et le rapport de données. Logstash permet aussi de réaliser des transformations de données puissantes.

#### Bad reviews 
* Le suivi des erreurs dans les données des journaux peut être difficile, et parfois des erreurs récurrentes font exploser les journaux d'erreurs.
* La documentation est parfois complète, mais il semble toujours y avoir des trous dans certains composants.
* Tarification : le niveau gratuit est excellent, mais pour intégrer des modules d'apprentissage automatique et la sécurité c’est payant.


### Roadmap  

La conférence officielle des utilisateurs Elasticsearch annonce de nombreux produits et roadmaps, ainsi que des avancements de machine learning et APM (Application Performance Monitoring) :

* Elasticsearch : Configuration de tâche périodiques qui « roll-up » ou pré-agrègent les données stockées dans un index et le rendent disponible à la recherche.
* Kibana : Nouvelles visualisations avec Canvas et amélioration des capacités de géolocalisation pour intégrer les cartes dans vos tableaux de bord.
* APM : Suivre et optimiser la performance de vos applications.
* Elastic Cloud et Elastic Cloud Enterprise : Flexibilité augmentée dans l’hébergement et la gestion des clusters
* X-Pack : Ouverture du code de X-Pack pour le rendre public. C’est une extension Elastic Stack qui fournit des fonctionnalités de sécurité, d'alerte, de surveillance, de création de rapports, d'apprentissage automatique et de nombreuses autres fonctionnalités.



