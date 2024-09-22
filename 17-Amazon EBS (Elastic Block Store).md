Amazon EBS fournit un stockage de blocs persistant utilisé avec Amazon EC2. EBS permet de créer des volumes de disques qui peuvent être attachés à des instances EC2 et sont idéaux pour les applications nécessitant un stockage rapide et à faible latence.

Caractéristiques principales :
Volumes de stockage de blocs : Les volumes EBS agissent comme des disques durs attachés aux instances EC2.
Haute disponibilité : Les volumes EBS sont répliqués dans une zone de disponibilité pour garantir la résilience.
Types de volumes :
General Purpose SSD (gp3) : Conçu pour les charges de travail générales qui nécessitent un bon équilibre entre coût et performance.
Provisioned IOPS SSD (io2) : Pour les applications nécessitant une très haute performance, comme les bases de données critiques.
Cold HDD (sc1) : Stockage à faible coût pour les données rarement accédées.
Throughput Optimized HDD (st1) : Idéal pour des applications qui nécessitent des accès séquentiels à grande échelle comme le traitement de gros volumes de données.
Cas d'usage :
Bases de données relationnelles et NoSQL : EBS est utilisé pour stocker les données d'applications comme MySQL, PostgreSQL, ou MongoDB.
Applications nécessitant une faible latence : Parfait pour des systèmes de gestion d'ERP, des systèmes de gestion transactionnelle ou des applications critiques avec des besoins de performance élevés.
Backup et snapshots : Les volumes EBS permettent de prendre des snapshots pour sauvegarder des volumes entiers ou migrer des données entre instances EC2.
