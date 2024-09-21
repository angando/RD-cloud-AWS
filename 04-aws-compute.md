
**les EC2 (Elastic Cloud Compute):**

**On-Demand EC2 Instances :**

Facturation : Le prix est fixé et facturé à la seconde.
Utilisation recommandée :
Lorsque les coûts sont faibles, sans paiements initiaux ni engagements.
Pour des charges de travail imprévisibles qui ne peuvent être interrompues.
Pour le développement d'applications.
Lorsque la charge de travail ne durera pas plus d'un an.


**Capacity Reservations :**

Utilisation : Réservations de capacité pour garantir une haute disponibilité, la reprise après sinistre, et l'assurance de la capacité.
Ces réservations maintiennent la capacité, que vous exécutiez ou non une instance.
En résumé, il s'agit de deux approches pour utiliser et gérer les ressources EC2 selon les besoins d'interruptibilité, de coût et de durée des charges de travail.



Imaginons une entreprise de développement de logiciels, DevSoft, qui crée une application mobile nécessitant un environnement cloud pour tester et déployer ses nouvelles versions.

Cas 1 : On-Demand EC2 Instances
DevSoft a besoin de tester des fonctionnalités de l’application, mais ces tests sont imprévisibles et ponctuels. L’équipe technique veut éviter des coûts élevés liés à des engagements à long terme, car les tests peuvent varier en durée, de quelques minutes à quelques heures. De plus, ils doivent s’assurer que les instances de calcul peuvent être facilement mises en marche et arrêtées sans engagements préalables.

Solution : Ils utilisent des instances On-Demand car elles offrent une flexibilité totale : la facturation est à la seconde, donc ils ne paient que pour le temps exact d’utilisation des instances. Cela permet à DevSoft de faire leurs tests sans coûts fixes et sans engagement de long terme, tout en adaptant leurs ressources en fonction des besoins du projet.
Cas 2 : Capacity Reservations
Parallèlement, DevSoft a un autre projet où ils doivent s'assurer d'une haute disponibilité pour une application critique de gestion de stock en temps réel. Cette application doit être toujours accessible car toute interruption pourrait impacter les ventes des clients. DevSoft a également des exigences strictes de reprise après sinistre, et ils ne peuvent pas se permettre une perte de capacité lors d'une augmentation soudaine de la charge.

Solution : Ils optent pour des Capacity Reservations afin de garantir la disponibilité des ressources nécessaires en cas de besoin. Même s’ils n'utilisent pas constamment les instances, la capacité est réservée pour eux, ce qui assure la stabilité de l’application critique, tout en respectant les exigences de haute disponibilité et de reprise après sinistre.
Ainsi, DevSoft utilise une combinaison des deux solutions pour gérer efficacement ses charges de travail : des instances On-Demand pour les tests flexibles à coût minimal, et des réservations de capacité pour garantir la continuité de leurs services critiques.




les instances On-Demand et les Capacity Reservations sont des concepts distincts, et ils ne sont pas forcément associés à la même instance EC2.

Voici les différences clés pour comprendre :
On-Demand Instances :

Lorsque vous utilisez une instance On-Demand, vous ne réservez pas une instance spécifique à l'avance. Vous lancez une instance EC2 et elle peut être créée sur n'importe quel hôte disponible dans la région ou la zone de disponibilité que vous avez choisie.
L'instance peut changer si vous l'arrêtez et la redémarrez, ou si vous en lancez une nouvelle. AWS attribue les ressources en fonction de la disponibilité au moment du lancement.
L'avantage est la flexibilité, mais il n'y a pas de garantie que la capacité sera disponible à un moment précis.
Capacity Reservations :

Avec Capacity Reservations, vous réservez de la capacité (i.e. des ressources spécifiques) dans une zone de disponibilité donnée, que vous utilisiez ou non l'instance. Cela garantit que la capacité est prête pour vous.
Cependant, cela ne signifie pas que vous réservez une instance EC2 spécifique, mais plutôt que vous avez une garantie que des instances avec les caractéristiques que vous avez spécifiées (par ex. type de machine, stockage) seront disponibles dans une zone donnée, même en cas de pic de demande.
Cela permet de s'assurer que si vous avez besoin d'une instance à un moment critique, elle sera disponible, contrairement aux instances On-Demand où il pourrait y avoir une pénurie temporaire de capacité.
