**Spot Instances :**

Utilisation : Elles exploitent les capacités EC2 non utilisées à un coût bien inférieur aux instances On-Demand.
Quand les utiliser :
Lorsque le démarrage ou l’arrêt des instances n’est pas critique.
Lorsqu'il est acceptable d'interrompre la charge de travail à tout moment.
Lorsque des prix de calcul très bas sont nécessaires.
C’est l’option la moins chère pour des besoins non critiques.
Avantage : Les Spot Instances permettent de réaliser des économies allant jusqu'à 90 % par rapport aux prix On-Demand. Le prix est fixé au début de chaque heure, en fonction de la capacité disponible.

Voici des cas d'usage concrets et avancés pour les Spot Instances :

Cas d’usage :
Traitement de données massives (Big Data) :

Les entreprises, comme celles dans les secteurs de l’analyse de données ou de la finance, effectuent souvent des traitements lourds de données qui n'ont pas besoin d'être continus. En utilisant des Spot Instances, elles peuvent exécuter des tâches comme des analyses prédictives, le traitement d'images ou la transformation de données ETL (Extract, Transform, Load), tout en minimisant les coûts.
Exemple concret : Une entreprise de marketing collecte des données clients en temps réel et utilise ces données pour exécuter des algorithmes de machine learning et d'analyse comportementale pendant la nuit, quand les interruptions n'affectent pas le service global. Ils lancent des Spot Instances pendant les heures de faible activité à des coûts très réduits.
Rendu vidéo et traitement graphique :

Le rendu de vidéos ou d’images 3D est un processus gourmand en ressources, mais qui peut tolérer des interruptions. Les studios d’animation, les architectes ou les entreprises de jeux vidéo peuvent lancer plusieurs instances de calcul simultanément en utilisant des Spot Instances.
Exemple concret : Un studio d'animation crée des films ou des publicités et doit traiter des rendus d'images en 3D. Ce processus peut durer des heures, voire des jours. En utilisant les Spot Instances, le studio peut faire fonctionner des centaines de machines pour rendre les images à un coût bien inférieur, tout en tolérant que certaines instances soient interrompues.
Tests de performance et simulations :

Les entreprises de logiciels ou les équipes DevOps peuvent utiliser des Spot Instances pour exécuter des tests de charge, des simulations ou des tests de résilience en masse. Ces tests peuvent être arrêtés et redémarrés sans impact, ce qui les rend parfaits pour une exécution sur des instances Spot.
Exemple concret : Une entreprise de services cloud effectue des tests de charge sur une nouvelle application pour voir combien de connexions simultanées leur infrastructure peut gérer. Ils utilisent des Spot Instances pour simuler des milliers de connexions utilisateur et ainsi réaliser ces tests à faible coût.
Rendering scientifique ou simulations :

Les chercheurs scientifiques qui exécutent des simulations complexes (par exemple, la modélisation climatique, les simulations moléculaires ou les études astrophysiques) ont besoin de puissance de calcul considérable. Bien que ces simulations soient importantes, les interruptions ne sont pas critiques pour la plupart d’entre elles, ce qui les rend idéales pour l’utilisation des Spot Instances.
Exemple concret : Un laboratoire universitaire effectue des simulations climatiques pour prédire l'évolution de la température terrestre. Ces simulations exigent une grande puissance de calcul, mais elles peuvent se permettre des arrêts temporaires. Utiliser des Spot Instances permet au laboratoire d'accomplir ses tâches avec des économies substantielles sur les coûts de calcul.
CI/CD (Intégration et Déploiement Continus) :

Les pipelines de CI/CD (Continuous Integration/Continuous Deployment) nécessitent parfois des ressources de calcul importantes pour compiler du code, exécuter des tests automatisés ou déployer des applications dans un environnement de staging. Ces tâches peuvent être exécutées via des Spot Instances pour diminuer les coûts tout en optimisant les processus de développement.
Exemple concret : Une entreprise de développement utilise Jenkins pour automatiser ses processus de déploiement. Ils configurent leur infrastructure CI/CD pour qu'elle s'exécute sur des Spot Instances, permettant à l’équipe de développer et tester en continu à un coût réduit, même si certaines instances sont interrompues et que le processus doit être redémarré.
