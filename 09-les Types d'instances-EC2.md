https://aws.amazon.com/fr/ec2/instance-types/


Types d'instances Amazon EC2

Types d'instances Amazon EC2 sont optimisées pour différentes tâches. Lors de la sélection d'un type d'instance, tenez compte des besoins spécifiques de vos charges de travail et applications. Cela peut inclure des exigences en matière de capacités de calcul, de mémoire ou de stockage.


**Instances à usage général:**
Les instances à usage général offrent un équilibre entre les ressources de calcul, de mémoire et de réseau. Vous pouvez les utiliser pour diverses charges de travail, telles que :

serveurs d'applications
serveurs de jeux
serveurs back-end pour applications d'entreprise
petites et moyennes bases de données
Supposons que vous disposez d'une application dans laquelle les besoins en ressources de calcul, de mémoire et de réseau sont à peu près équivalents. Vous pouvez envisager de l'exécuter sur une instance à usage général, car l'application ne nécessite aucune optimisation dans un seul domaine de ressources.


**instances optimisées pour le calcul:**
Les instances optimisées pour le calcul sont idéales pour les applications de calcul qui bénéficient de processeurs hautes performances. Comme les instances à usage général, vous pouvez utiliser des instances optimisées pour le calcul pour des charges de travail telles que des serveurs Web, d'applications et de jeux.
Cependant, la différence réside dans le fait que les applications optimisées en termes de calcul sont idéales pour les serveurs Web hautes performances, les serveurs d'applications à calcul intensif et les serveurs de jeu dédiés. Vous pouvez également utiliser des instances optimisées en termes de calcul pour les charges de travail de traitement par lots qui nécessitent le traitement de nombreuses transactions dans un seul groupe.


**Instances optimisées en mémoire**:
Les instances optimisées en mémoire sont conçues pour offrir des performances rapides aux charges de travail qui traitent de grands ensembles de données en mémoire. En informatique, la mémoire est une zone de stockage temporaire. Elle contient toutes les données et instructions dont une unité centrale de traitement (CPU) a besoin pour pouvoir exécuter des actions. Avant qu'un programme ou une application informatique ne puisse s'exécuter, il est chargé du stockage vers la mémoire. Ce processus de préchargement donne au processeur un accès direct au programme informatique.
Supposons que vous ayez une charge de travail qui nécessite le préchargement de grandes quantités de données avant l'exécution d'une application. Ce scénario peut être une base de données hautes performances ou une charge de travail qui implique le traitement en temps réel d'une grande quantité de données non structurées. Dans ces types de cas d'utilisation, envisagez d'utiliser une instance optimisée en mémoire. Les instances optimisées en mémoire vous permettent d'exécuter des charges de travail avec des besoins en mémoire élevés et de bénéficier de performances exceptionnelles.



La différence entre les instances optimisées pour le calcul et les instances optimisées en mémoire réside dans les types de charges de travail qu'elles sont conçues pour gérer :

Instances optimisées pour le calcul :
Ces instances sont idéales pour les applications de calcul intensif qui nécessitent une grande puissance de traitement des processeurs.
Elles conviennent particulièrement aux serveurs Web hautes performances, aux serveurs d'applications nécessitant beaucoup de calculs, et aux serveurs de jeu dédiés.
Elles sont également utilisées pour des charges de travail qui nécessitent le traitement par lots de nombreuses transactions simultanées, comme des calculs scientifiques, des simulations, et des modèles financiers complexes.
En résumé, les instances optimisées pour le calcul sont axées sur les performances du CPU, et elles sont adaptées aux charges de travail qui nécessitent une grande puissance de traitement.
Instances optimisées en mémoire :

Ces instances sont conçues pour des charges de travail qui nécessitent beaucoup de mémoire et où les données doivent être traitées rapidement en mémoire.
Elles sont idéales pour des applications qui traitent de grands ensembles de données en mémoire, comme les bases de données hautes performances ou le traitement en temps réel de données non structurées.
Le but principal des instances optimisées en mémoire est de permettre un accès rapide aux données par le processeur une fois que celles-ci sont préchargées en mémoire, offrant ainsi des performances exceptionnelles pour des charges de travail qui exploitent fortement la mémoire vive (RAM).
En résumé, ces instances sont axées sur la quantité et la rapidité de la mémoire, et sont adaptées aux applications nécessitant un grand volume de données en mémoire,
comme les bases de données en mémoire, le caching, et les gros traitements de données.


**Instances de calcul accélérées:**
Les instances de calcul accéléré utilisent des accélérateurs matériels, ou coprocesseurs, pour exécuter certaines fonctions plus efficacement que ce qui est possible dans les logiciels exécutés sur des processeurs. Parmi ces fonctions, on peut citer les calculs de nombres à virgule flottante, le traitement graphique et la correspondance de modèles de données.
En informatique, un accélérateur matériel est un composant qui peut accélérer le traitement des données. Les instances de calcul accéléré sont idéales pour les charges de travail telles que les applications graphiques, le streaming de jeux et le streaming d'applications.

**Instances optimisées pour le stockage:**
Les instances optimisées pour le stockage sont conçues pour les charges de travail qui nécessitent un accès séquentiel élevé en lecture et en écriture à de grands ensembles de données sur le stockage local. Les exemples de charges de travail adaptées aux instances optimisées pour le stockage incluent les systèmes de fichiers distribués, les applications d'entreposage de données et les systèmes de traitement de transactions en ligne à haute fréquence (OLTP).
En informatique, le terme « opérations d'entrée/sortie par seconde » (IOPS) est une mesure qui mesure les performances d'un périphérique de stockage. Il indique le nombre d'opérations d'entrée ou de sortie différentes qu'un périphérique peut effectuer en une seconde. Les instances optimisées pour le stockage sont conçues pour fournir des dizaines de milliers d'IOPS aléatoires à faible latence aux applications. 
Vous pouvez considérer les opérations d'entrée comme des données introduites dans un système, telles que des enregistrements saisis dans une base de données. Une opération de sortie correspond à des données générées par un serveur. Un exemple de sortie peut être l'analyse effectuée sur les enregistrements d'une base de données. Si vous avez une application qui a des besoins élevés en IOPS, une instance optimisée pour le stockage peut offrir de meilleures performances que d'autres types d'instances non optimisés pour ce type de cas d'utilisation.
