**Explication des concepts clés :**
Savings Plans :

Un engagement à utiliser des ressources de calcul pour une période allant de 1 à 3 ans. L'utilisation est calculée à l'heure.
Ce plan permet une réduction allant jusqu'à 72 % des prix On-Demand (tarification à l'usage sans engagement).
Flexibilité : Les utilisateurs peuvent changer de services de calcul, de types d'instances, de systèmes d'exploitation ou de régions, tout en continuant à bénéficier de tarifs réduits.

Contrairement aux Reserved Instances, il n'y a pas de réservation de capacité (ce qui signifie que l'utilisateur ne bloque pas des instances spécifiques, mais bénéficie de tarifs réduits en fonction de son engagement global en termes d'heures de calcul).
Cas d'usage pour Savings Plans :

Exemple 1 : Optimisation des coûts sur plusieurs services AWS : Une entreprise qui utilise à la fois des instances EC2 pour ses serveurs web et des services de calcul via AWS Lambda pour des traitements sans serveur peut choisir un Savings Plan. Elle réduit ainsi ses coûts sur l'ensemble de ses services de calcul, tout en conservant la flexibilité de migrer ses workloads entre différents services selon ses besoins.

Exemple 2 : Entreprise avec des besoins fluctuants : Une société qui déploie ses instances sur différentes régions du monde en fonction de la demande saisonnière peut choisir un Savings Plan pour éviter les coûts élevés de l'On-Demand tout en conservant la flexibilité de déplacer ses ressources dans des régions géographiques différentes.

Exemple 3 : Utilisation de différentes configurations : Une entreprise qui change régulièrement de types d'instances pour des raisons de performance ou de coût, comme par exemple passer de machines t2.medium à des machines plus puissantes comme c5.large, pourrait bénéficier de cette flexibilité tout en réduisant ses coûts.

Différences entre Savings Plans et Reserved Instances :

Les Reserved Instances permettent également des réductions, mais elles sont liées à des instances spécifiques (type, région, durée), et elles nécessitent souvent de réserver une capacité à l'avance.
Avec les Savings Plans, il est possible d'appliquer les économies à différents services et régions sans être limité à des instances spécifiques. Cela offre plus de souplesse tout en maintenant des économies importantes.
