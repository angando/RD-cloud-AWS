AWS Database Migration Service (DMS) est un service entièrement managé qui facilite la migration des bases de données vers AWS. Il permet de migrer des bases de données tout en assurant que celles-ci restent opérationnelles pendant le processus, ce qui minimise les interruptions de service. DMS prend en charge les migrations entre bases de données homogènes (ex: Oracle vers Oracle) et hétérogènes (ex: Oracle vers MySQL), et il permet également des réplications continues pour maintenir la synchronisation entre la source et la destination.

Caractéristiques principales d’AWS DMS :
Migrations homogènes et hétérogènes :

Migrations homogènes : Migration de bases de données du même type, par exemple MySQL vers MySQL, Oracle vers Oracle, etc.
Migrations hétérogènes : Migration entre des bases de données différentes, par exemple Oracle vers Amazon Aurora, SQL Server vers PostgreSQL, ou Oracle vers MySQL. Dans ces cas, il est souvent nécessaire de convertir le schéma de la base de données à l'aide de AWS Schema Conversion Tool (SCT).
Migration en temps réel avec réplication continue :

DMS prend en charge la réplication continue des données, ce qui signifie que la base de données source peut continuer à fonctionner pendant la migration. Cela permet d'éviter des temps d’arrêt prolongés, car la base de données cible est mise à jour en temps réel.
Conversion automatique des schémas (AWS SCT) :

Lors de migrations hétérogènes, AWS Schema Conversion Tool (SCT) est utilisé pour convertir automatiquement les schémas de la base de données source en un schéma compatible avec la base de données cible. SCT prend en charge les conversions entre des bases de données commerciales et des bases de données open-source telles que PostgreSQL ou MySQL.
Support des bases de données relationnelles et NoSQL :

AWS DMS prend en charge une large gamme de bases de données, y compris des bases de données relationnelles (MySQL, PostgreSQL, SQL Server, Oracle, etc.), des bases de données NoSQL (Amazon DynamoDB), ainsi que des entrepôts de données (Amazon Redshift).
Migration flexible et évolutive :

DMS peut migrer des bases de données de petite ou grande taille, et il est capable de s'adapter à des charges de travail croissantes. Le service permet également la migration incrémentale, ce qui signifie que seules les modifications apportées après le démarrage de la migration sont appliquées à la base de données cible.
Surveillance intégrée :

AWS DMS intègre des outils de surveillance via Amazon CloudWatch, permettant de suivre l'état de la migration en temps réel. Les métriques incluent la progression de la migration, les temps de latence, les taux de transfert de données, et plus encore.
Tolérance aux pannes :

DMS est conçu pour être tolérant aux pannes, ce qui signifie que même si une panne survient pendant la migration, le service reprend automatiquement la migration là où elle s'était arrêtée sans perte de données.
Cas d’usage d’AWS DMS :
Migration vers le cloud :

DMS est largement utilisé pour migrer des bases de données on-premise vers le cloud AWS. Par exemple, une entreprise utilisant Oracle dans ses propres datacenters peut migrer ses données vers Amazon RDS for Oracle ou une base de données Aurora.
Modernisation des bases de données :

Pour les entreprises cherchant à moderniser leurs infrastructures, DMS permet de migrer des bases de données commerciales coûteuses vers des alternatives open-source telles que Amazon Aurora, PostgreSQL, ou MySQL. Cela permet de réduire les coûts tout en profitant des avantages des bases de données cloud natives.
Consolidation des bases de données :

Les organisations qui possèdent plusieurs bases de données disparates peuvent utiliser DMS pour les consolider dans une seule base de données ou un entrepôt de données, tel que Amazon Redshift. Cela permet une gestion plus facile des données et des analyses consolidées.
Migration vers des bases de données NoSQL :

DMS peut également être utilisé pour migrer des bases de données relationnelles vers NoSQL, comme Amazon DynamoDB, lorsque les entreprises souhaitent profiter de la scalabilité et des performances des bases de données NoSQL pour certaines charges de travail.
Réplication et synchronisation continues :

DMS permet de mettre en place des systèmes de réplication en temps réel pour des scénarios de sauvegarde, de réplication de données dans plusieurs régions AWS, ou pour synchroniser des bases de données entre des environnements sur site et des environnements cloud.
Environnements hybrides :

Pour les entreprises qui maintiennent des environnements hybrides, AWS DMS permet de synchroniser les bases de données entre un datacenter sur site et des instances cloud. Cela est utile pour les environnements où une migration complète vers le cloud n'est pas encore envisageable, mais où une synchronisation des données est nécessaire.
Étapes de migration avec AWS DMS :
Préparation de la source et de la cible :

Choisissez la base de données source (par exemple, un serveur Oracle sur site) et la base de données cible (par exemple, Amazon Aurora sur AWS). Si vous réalisez une migration hétérogène, utilisez AWS Schema Conversion Tool (SCT) pour convertir les schémas de la source vers la cible.
Configuration de la tâche de migration :

Dans la console AWS DMS, configurez la tâche de migration. Cela implique de spécifier les endpoints de la base de données source et de la base de données cible, ainsi que de définir les options de migration, comme la réplication continue ou la migration de données en une seule fois.
Lancement de la migration :

Démarrez la tâche de migration. AWS DMS commencera à transférer les données de la base source vers la base cible. Pendant ce temps, les applications peuvent continuer à interagir avec la base de données source.
Surveillance et ajustements :

Utilisez Amazon CloudWatch pour surveiller l'état de la migration, y compris les éventuelles erreurs ou latences. Les ajustements peuvent être faits en temps réel pour optimiser le processus.
Réplication continue (si nécessaire) :

Une fois la migration initiale terminée, vous pouvez configurer la réplication continue pour synchroniser les modifications en cours entre la source et la cible. Cela permet de basculer vers la nouvelle base de données sans interruption de service.
Validation et bascule :

Une fois la migration terminée et validée, vous pouvez basculez votre application vers la base de données cible.
Avantages d’AWS DMS :
Minimalisation des interruptions :

Avec la réplication continue, la base de données source reste opérationnelle pendant toute la durée de la migration, réduisant ainsi les interruptions de service.
Flexibilité :

DMS prend en charge une large gamme de bases de données relationnelles et NoSQL, ainsi que des environnements sur site, AWS, et hybrides.
Automatisation et tolérance aux pannes :

DMS est tolérant aux pannes et reprend automatiquement la migration après une interruption, ce qui réduit les risques associés aux migrations manuelles.
Réduction des coûts :

La migration des bases de données vers le cloud AWS permet de réduire les coûts opérationnels liés à la gestion de bases de données sur site, tout en profitant des avantages de la scalabilité et des fonctionnalités managées d’AWS.
Rapidité de mise en œuvre :

DMS simplifie et accélère le processus de migration, même pour les charges de travail volumineuses et critiques, avec peu ou pas de temps d'arrêt.
