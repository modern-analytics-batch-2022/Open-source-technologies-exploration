# Flink Technology
### Brief description :
Apache Flink est un cadre de traitement de flux open source avec de puissantes capacités de traitement de flux et par lots.
Flink a été conçu pour fonctionner dans tous les environnements de cluster communs, effectuer des calculs à la vitesse en mémoire et à n’importe quelle échelle.
Flink est un moteur de traitement distribué et un cadre d’analyse des données évolutif.
![](https://flink.apache.org/img/flink-home-graphic.png)
### General information :
##### Creation year :
Flink a été créé en  mai 2011
##### Website :
le site officiel de Flink est : [https://flink.apache.org/](https://flink.apache.org/)
##### Github repo :
le répertoire de Flink est : [https://github.com/apache/flink](https://github.com/apache/flink)
##### Community channel :
Voici le canal communautaire de Flink : [https://flink.apache.org/community.html](https://flink.apache.org/community.html)
##### Communiy size :
En 2015, la communauté de Flink a doublé de taille, passant d’environ 75 contributeurs à plus de 150. Les fourches du répertoire ont plus que triplé, passant de 160 en février 2015 à 544 en décembre 2015, et le nombre d’étoiles du répertoire a presque triplé, passant de 289 à 813.
##### Founders :
Apache Flink est un projet open source de **The Apache Software Foundation (ASF)**. Le projet Apache Flink est issu du projet de **recherche Stratosphere**.
### Main capabilities:
-  Vous pouvez utiliser Flink pour traiter des flux de données à grande échelle et pour fournir des informations analytiques en temps réel sur vos données traitées avec votre application de streaming.
-   Bibliothèques pour le traitement graphique (par lots), l’apprentissage automatique (par lots) et le traitement d’événements complexes (diffusion en continu/streaming).
-   Vous pouvez utiliser Flink pour les microservices événementiels (event driven), l’analyse de données ou les pipelines de données pour ETL et bien d’autres. Vous pouvez écrire des programmes simples pour traiter et agréger des flux de données en temps réel, pas besoin d’écrire des tâches par lots.
-   Gestion de la mémoire personnalisée pour une commutation efficace et robuste entre la mémoire interne et les algorithmes de traitement des données hors cœur.
-   Si vous avez besoin de faire un traitement de flux complexe, alors l’utilisation d’Apache Flink serait fortement recommandée.
-    Couches de compatibilité pour Apache Hadoop MapReduce.
-    Intégration avec YARN, HDFS, HBase et d’autres composants de l’écosystème Apache Hadoop.
-    Un environnement d'exécution *streaming-first* qui prend en charge à la fois le traitement par lots et les programmes de flux de données.

### Available Connectors / Integrations :
##### Connectors :
- 	Apache Kafka (source/sink).
- 	Apache Cassandra (sink).
- 	Amazon Kinesis Streams (source/sink).
-	Elasticsearch (sink).
-	FileSystem (sink).
-	RabbitMQ (source/sink).
-	Google PubSub (source/sink).
-	Hybrid Source (source).
-	Apache NiFi (source/sink).
-	Apache Pulsar (source).
-	JDBC (sink).

##### Integrations :
-   Apache Kafka.
-	Amazon Kinesis Streams.
-	RabbitMQ.
-	Apache NiFi.
-	Twitter Streaming API.

###	Ways to deploy it :
-  	*On-prem (Local)* : Exécutez Flink localement pour les tests de base et l’expérimentation.
-  	*Standalone* : Une solution simple pour le fonctionnement de Flink sur métal nu ou sur VM.
-  	*Yarn* : Déployez Flink au-dessus du gestionnaire de ressources d’Apache Hadoop.
-  	*Mesos* : Un gestionnaire de ressources générique pour l’exécution de systèmes distriubted
-   *Docker* : Une solution populaire pour faire fonctionner Flink dans un environnement conteneurisé.
-   *Kubernetes* : Un système automatisé pour le déploiement d’applications conteneurisées.

### Reviews :
##### Good reviews :
1. Flink a une note globale de 3,9 sur 5, basée sur plus de 37 avis laissés anonymement par les employés. 81 % des employés recommanderaient de travailler chez Flink à un ami et 69 % ont une perspective positive pour l’entreprise. Cette note est stable depuis 12 mois.
2. Une autre caractéristique est la façon dont Flink gère ses rayons. Il a quelque chose appelé le concept de **checkpointing**. Vous traitez des milliards et des milliards de demandes, donc votre système va tomber en panne dans les grands systèmes de stockage. Flink gère cela en utilisant le concept de **checkpointing** et **savepointing**, où ils écrivent l’état agrégé dans un stockage séparé. Donc, en cas d’échec, vous pouvez essentiellement vous rappeler de cet état et revenir.

##### Bad reviews :
- Pour ce qui est de la stabilité avec Flink, c’est quelque chose que vous devez gérer à chaque fois. La stabilité est le problème numéro un que nous avons vu avec Flink, et cela dépend vraiment du genre de problème que vous essayez de résoudre.

### Roadmap :
![Flink road map](https://flink.apache.org/img/flink_feature_radar_2.svg)
