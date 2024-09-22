Les coûts d'AWS Fargate et d'AWS Lambda fonctionnent différemment en raison de la nature des services. Voici une comparaison détaillée de leurs modèles de facturation :

1. Modèle de facturation AWS Lambda
Facturation à l’utilisation : AWS Lambda est facturé en fonction du nombre de requêtes et du temps d'exécution de vos fonctions.

Nombre de requêtes : Vous êtes facturé pour chaque appel à une fonction Lambda. Le premier million de requêtes par mois est gratuit, puis il y a un coût pour chaque requête supplémentaire.

Temps d'exécution : La facturation repose sur la durée pendant laquelle votre code s'exécute, calculée en millisecondes. Le prix dépend de la quantité de mémoire allouée à la fonction, qui varie de 128 Mo à 10 Go. Plus la mémoire allouée est importante, plus le coût est élevé.

Exemple de coût Lambda :

Vous payez uniquement pour le temps d'exécution exact. Par exemple, si une fonction Lambda avec 512 Mo de mémoire allouée s'exécute pendant 1 seconde, vous serez facturé pour cette durée précise.
Gratuité : Lambda propose un tiers gratuit qui inclut 1 million de requêtes gratuites et 400 000 Go-seconde d'exécution par mois.

2. Modèle de facturation AWS Fargate
Facturation basée sur les ressources allouées : Contrairement à Lambda, AWS Fargate facture en fonction des ressources de calcul (CPU et mémoire) que vous allouez à vos conteneurs.

VCPU et Mémoire : Fargate facture en fonction du nombre de vCPU (virtual CPU) et de la mémoire allouée à une tâche ou à un pod. Le coût est calculé à la seconde à partir du moment où les conteneurs commencent à s’exécuter jusqu'à ce qu'ils soient arrêtés.

Exemple de coût Fargate :

Si vous exécutez une tâche avec 1 vCPU et 2 Go de mémoire pendant 1 heure, vous serez facturé pour cette combinaison de vCPU et de mémoire allouée, même si la tâche ne consomme pas 100 % de ces ressources.
Pas de gestion des serveurs : Contrairement aux clusters EC2 gérés par vous-même, avec Fargate vous ne payez pas pour les instances EC2 mais uniquement pour les conteneurs déployés. Cela simplifie la gestion, mais peut être plus coûteux pour des charges de travail à long terme ou intensives.

Comparaison des coûts
AWS Lambda est idéal pour des tâches courtes et des exécutions qui n'ont pas besoin de fonctionner en permanence. Le modèle de facturation étant basé sur le nombre de requêtes et la durée d’exécution, il est plus économique pour des workloads irréguliers ou à faible volume. Les microservices, les automatisations basées sur des événements, et les petites API peuvent être très rentables avec Lambda.

AWS Fargate est souvent utilisé pour des charges de travail conteneurisées de plus longue durée et qui nécessitent des configurations spécifiques de CPU et de mémoire. Les applications complexes ou microservices à grande échelle avec des besoins de conteneurisation sont mieux adaptées à Fargate, car il offre plus de flexibilité sur la gestion des ressources, bien que son coût puisse être plus élevé pour les applications fonctionnant en permanence.

Quels types d’usage sont les plus rentables ?
Lambda : Si vous avez des fonctions courtes, peu fréquentes ou irrégulières, Lambda est généralement plus rentable grâce à la facturation ultra-granulaire. C'est souvent le choix idéal pour les tâches serverless, comme l'exécution de scripts ou d'API à faible demande.

Fargate : Si vous avez des charges de travail longues, telles que des applications web qui doivent être actives en permanence ou des tâches nécessitant plus de contrôle sur la gestion des ressources CPU et mémoire, Fargate devient plus rentable, car Lambda peut devenir coûteux si le temps d'exécution devient élevé.

Résumé des coûts Lambda vs Fargate
Lambda :

Pay-per-request (facturation à la requête).
Coût basé sur le temps d'exécution.
Tiers gratuit généreux (1 million de requêtes par mois).
Idéal pour des charges de travail courtes et irrégulières.
Fargate :

Pay-per-resource (facturation basée sur CPU/mémoire alloués).
Coût à la seconde d'exécution, basé sur les ressources allouées (vCPU et mémoire).
Idéal pour des charges de travail plus longues et complexes nécessitant une gestion fine des ressources.


En conclusion, AWS Lambda est plus rentable pour des workloads ponctuels et événementiels, tandis que Fargate est mieux adapté aux applications conteneurisées à plus grande échelle ou nécessitant une allocation précise des ressources CPU/mémoire.
