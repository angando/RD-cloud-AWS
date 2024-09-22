L’EC2 Instance Store est un type de stockage temporaire qui est directement attaché à une instance Amazon EC2. Contrairement à Amazon EBS (Elastic Block Store), qui offre un stockage persistant et redondant, l'instance store est éphémère, ce qui signifie que les données sont perdues lorsque l'instance est arrêtée, redémarrée ou terminée.

Caractéristiques principales de l'EC2 Instance Store :
Stockage éphémère :

Les volumes de l’instance store ne sont disponibles que pendant la durée de vie de l'instance EC2. Lorsque vous éteignez ou redémarrez l'instance, toutes les données sur ces volumes sont perdues.
Les données restent disponibles uniquement tant que l'instance EC2 continue de fonctionner.
Attache locale au serveur hôte :

Contrairement à Amazon EBS, qui est un stockage réseau séparé, l'instance store est attaché localement à l'hôte physique où l'instance EC2 s'exécute. Cela offre des performances d'entrée/sortie plus rapides pour certaines charges de travail.
La latence est généralement plus faible qu'avec EBS, car le stockage est local à l'instance.
Volumes temporaires très rapides :

L'instance store offre des performances élevées en termes de lecture/écriture. Ce type de stockage est optimal pour des applications nécessitant un stockage rapide mais non persistant, comme les bases de données en mémoire, les caches temporaires, ou les fichiers temporaires dans des environnements à haute performance.
Capacité limitée :

La capacité du volume d’instance store dépend du type d’instance EC2 choisi. Certaines instances offrent plusieurs téraoctets de stockage local (par exemple, les instances i3), tandis que d'autres offrent peu ou pas de stockage local.
Pas de coût supplémentaire :

Le stockage instance store est inclus dans le coût de l'instance EC2, vous ne payez donc pas de supplément pour les volumes d'instance store. Cependant, il n’offre pas la flexibilité de l'allocation séparée comme EBS.
Cas d'usage de l'EC2 Instance Store :
Caches temporaires :

Applications de cache : Le stockage instance store est parfait pour des caches temporaires où les données peuvent être régénérées ou récupérées à partir d'une source primaire en cas de défaillance. Par exemple, des caches de fichiers ou des données calculées peuvent être stockés localement pour accélérer les performances sans besoin de persistance.
Stockage de fichiers temporaires :

Dans des scénarios de traitement de fichiers temporaires, comme le traitement vidéo ou image, ou des simulations nécessitant beaucoup de calculs, l'instance store permet de stocker temporairement des fichiers intermédiaires avant leur archivage dans un stockage persistant comme S3.
Applications nécessitant un IOPS élevé :

Certaines charges de travail qui nécessitent un très grand nombre d'opérations d'entrée/sortie par seconde (IOPS) peuvent bénéficier de l'instance store, comme les bases de données en mémoire (in-memory databases), les big data ou les pipelines de traitement de données.
Environnements de développement et de test :

Les environnements de développement où les données ne nécessitent pas d’être conservées de manière persistante peuvent utiliser l'instance store pour effectuer des tests rapides, sans coûts supplémentaires.
Bases de données NoSQL temporaires :

Les bases de données temporaires qui peuvent être régénérées, comme Redis ou Memcached, utilisent souvent l'instance store pour son faible temps de latence et ses performances élevées.

Cas d’usage à éviter avec Instance Store :
Applications nécessitant une persistance des données :

Si vous devez stocker des données critiques et garantir leur persistance (par exemple, des bases de données relationnelles comme MySQL ou PostgreSQL), il est préférable d'utiliser des volumes EBS ou EFS qui offrent des sauvegardes automatiques et une redondance.
Applications avec besoin de réplication inter-AZ :

L'instance store ne permet pas de répliquer les données sur plusieurs zones de disponibilité (AZ), donc pour des données critiques nécessitant une haute disponibilité et une réplication, Amazon S3 ou EBS sont plus adaptés.
Conclusion :
L'EC2 Instance Store est un excellent choix pour des applications qui nécessitent un stockage rapide et éphémère, comme des caches ou des fichiers temporaires. Il offre des performances élevées, car les données sont stockées localement sur le matériel sous-jacent de l'instance EC2. Cependant, ce type de stockage doit être utilisé avec précaution pour des tâches non critiques, car les données sont perdues si l'instance est arrêtée. Pour les charges de travail nécessitant une persistance des données et une haute disponibilité, des solutions comme Amazon EBS ou S3 sont préférables.







