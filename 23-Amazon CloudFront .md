**1. Amazon CloudFront : Le service CDN principal d'AWS**
Amazon CloudFront est un réseau de diffusion de contenu qui délivre des données, des vidéos, des applications, et des API à des utilisateurs du monde entier avec des temps de latence réduits et des vitesses de transfert élevées. Il repose sur un réseau mondial de serveurs de cache situés dans des emplacements périphériques (Edge Locations).

***Caractéristiques principales :***
Caches mondiaux : CloudFront dispose de plusieurs emplacements périphériques à travers le monde. Lorsqu'un utilisateur fait une requête pour du contenu (par exemple une page web, une vidéo, ou une image), cette requête est redirigée vers l’emplacement le plus proche de l’utilisateur, réduisant ainsi la latence.
Intégration avec S3, EC2, et autres services AWS : CloudFront fonctionne en synergie avec d'autres services AWS comme Amazon S3, EC2, ou Elastic Load Balancing pour accélérer la distribution des contenus stockés ou hébergés sur AWS.
Sécurité intégrée : Il prend en charge l'intégration avec AWS Shield, AWS Web Application Firewall (WAF), et AWS IAM pour sécuriser les contenus contre les attaques DDoS, les intrusions, et garantir l’accès authentifié aux ressources.
Streaming vidéo et distribution de contenu dynamique : CloudFront permet de diffuser des vidéos en streaming en direct ou à la demande avec un support pour des formats de vidéo modernes comme HLS et MPEG-DASH.
Prise en charge HTTPS : Assure que les données sont transmises en toute sécurité avec le chiffrement SSL/TLS pour protéger les données sensibles.
Cas d’usage :
Streaming vidéo en direct :

CloudFront est souvent utilisé pour distribuer des vidéos en direct à des millions d’utilisateurs partout dans le monde. Son intégration avec des services comme AWS Elemental MediaLive et MediaPackage le rend idéal pour le streaming d'événements en direct.
Accélération de sites web et d'applications :

Les entreprises utilisent CloudFront pour diffuser des pages web statiques et dynamiques avec une latence minimale. Par exemple, les sites de commerce électronique ou les applications en ligne critiques qui nécessitent un temps de réponse rapide tirent parti de CloudFront pour améliorer l'expérience utilisateur.
Distribution de contenu mondial :

Les entreprises qui hébergent des applications mondiales (comme des jeux en ligne, des portails d’actualités, ou des plateformes sociales) utilisent CloudFront pour servir du contenu rapidement et de manière fiable aux utilisateurs, quel que soit leur emplacement géographique.
Protection contre les attaques DDoS :

CloudFront, associé à AWS Shield, est souvent utilisé pour sécuriser des sites web et des API contre des attaques par déni de service (DDoS). Il peut également bloquer des requêtes malveillantes grâce à l'intégration avec AWS WAF.
