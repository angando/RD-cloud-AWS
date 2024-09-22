AWS Storage Gateway est un service hybride qui permet de connecter votre infrastructure locale au cloud AWS, en utilisant le stockage AWS comme extension de vos systèmes de stockage locaux. Cela vous permet d'accéder et d'intégrer de manière transparente vos données locales avec AWS, offrant ainsi des solutions de sauvegarde, d'archivage, et de récupération. Ce service est conçu pour répondre aux besoins des entreprises souhaitant bénéficier des avantages du cloud tout en conservant leurs environnements locaux.

Les trois types de Storage Gateway :
File Gateway :

Fonctionnement : File Gateway permet d'accéder à vos fichiers locaux via des protocoles NFS (Network File System) et SMB (Server Message Block). Les fichiers sont ensuite convertis en objets et stockés directement dans Amazon S3.
Utilisation : Cela permet de conserver l'accès aux fichiers sur site tout en utilisant S3 pour les sauvegardes ou l'archivage, sans avoir à modifier les applications existantes.
Volume Gateway :

Fonctionnement : Volume Gateway crée des volumes de stockage locaux, qui sont ensuite sauvegardés de façon incrémentielle dans AWS sous forme de snapshots EBS (Elastic Block Store). Vous pouvez choisir entre deux modes :
Gateway-cached : Vos données principales sont stockées dans AWS, mais les données les plus fréquemment utilisées sont mises en cache localement.
Gateway-stored : Vos données sont principalement stockées localement, avec des sauvegardes automatiques dans AWS.
Utilisation : Cela est idéal pour les entreprises qui souhaitent conserver leurs données principales localement tout en assurant une sauvegarde automatisée et sécurisée dans AWS.
Tape Gateway :

Fonctionnement : Tape Gateway virtualise les bandes physiques d'archivage en les stockant dans Amazon S3 ou Amazon Glacier (pour l'archivage à long terme à faible coût). Vos processus de sauvegarde basés sur des bandes ne nécessitent pas de modifications.
Utilisation : C'est une solution idéale pour les entreprises qui utilisent encore des bandes physiques pour leurs archives et qui souhaitent passer à une gestion numérique sans modifier leurs flux de travail existants.
Cas d’usage de AWS Storage Gateway :
Extension des systèmes de stockage locaux :

Si votre infrastructure locale est limitée en termes de capacité de stockage, AWS Storage Gateway vous permet d'augmenter cette capacité en la connectant à AWS. Cela vous permet de gérer plus de données tout en continuant à utiliser vos processus de stockage traditionnels.
Migration vers le cloud :

Pour les entreprises souhaitant migrer leurs données vers le cloud de manière progressive, Storage Gateway permet une transition en douceur en stockant certaines données localement tout en utilisant AWS pour l'archivage et la sauvegarde. Vous pouvez déplacer des parties de vos données vers le cloud sans perturber votre infrastructure existante.
Sauvegarde et récupération :

AWS Storage Gateway simplifie la sauvegarde et la récupération en permettant de sauvegarder automatiquement vos données dans le cloud. Cela offre des copies sécurisées et automatisées des données locales, avec une option de restauration rapide en cas de besoin, qu'il s'agisse de données actives ou archivées.
