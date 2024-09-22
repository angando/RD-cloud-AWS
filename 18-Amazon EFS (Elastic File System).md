Amazon EFS est un système de fichiers géré et évolutif pour les instances EC2. EFS fournit un stockage de type NFS (Network File System) accessible par plusieurs instances simultanément et qui s'adapte automatiquement aux besoins de stockage.

Caractéristiques principales :
Stockage de fichiers : EFS permet le partage de fichiers entre plusieurs instances EC2.
Scalabilité automatique : Le système de fichiers s’adapte automatiquement à l'augmentation ou à la réduction des données sans intervention manuelle.
Multi-AZ : EFS réplique automatiquement les données dans plusieurs zones de disponibilité pour une haute disponibilité.
Performances :
Standard : Performances adaptées à la plupart des applications générales.
Infrequent Access (IA) : Pour les données moins fréquemment consultées, offrant un coût inférieur.
Cas d'usage :
Applications distribuées : Idéal pour les systèmes où plusieurs instances doivent accéder aux mêmes fichiers, comme des environnements de développement ou de test partagés.
Applications web : Parfait pour des applications web ou des sites qui ont besoin d'un accès rapide aux fichiers partagés, comme les serveurs web.
Big data et analyse : EFS peut être utilisé comme stockage de fichiers dans des environnements d'analyse de données qui nécessitent une lecture et écriture simultanées à grande échelle.
