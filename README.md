# Installation de Spiceworks

#### Contexte

Ce projet est un laboratoire effectué dans un project scolaire.

Pour ce projet, j'ai 3 serveurs qui doivent être monitoré. Dont un serveur sous Linux, un serveur W2k16 Core et un Windows server 2012 R2 où est installé notre outil de monitoring.

Nous possédons une instance EC2 chez Amazon, c'est sur cette dernière que nous effectuons une connexion en utilisant un tunnel SSH. Une fois la connexion établie, nous pouvons soit se connecter en SSH pour notre serveur Linux sous Centos ou en RDP sur nos serveurs Windows.

Le service Mysql \(Centos\) ainsi que le service Files sur le server Core doivent être monitorer également.

Le temps que nous avions à disposition pour conclure ce projet est de : 

#### Prérequis Serveur

| SPEC |  |
| :--- | :--- |
| OS | 64-bit Windows - Win Server 2012 R2 |
| CPU | Dual-core CPU |
| RAM | 4GB |
| Disque | At least 50 GB |

#### Dépendance 

Le firmware .NET 4.5 est nécessaire pour l'installation de cette solution, ainsi qu'une connexion internet active. 

#### Sécurité

![](.gitbook/assets/image.png)

* 4094 - collector service
* 5555 - Processor service
* 6739 - redis database
* 8005 - app server
* 8009 - app server

#### Mise en place 

Pour l'installation de l'outil de monitoring Spiceworks, nous devons tout d'abord nous connecter en remote sur notre serveur. 

Une fois la connexion établie, nous devons nous rendre sur le site de Spiceworks pour télécharger l'exécutable. 

{% embed url="https://www.spiceworks.com/download/monitor" %}

Suite au téléchargement de ce dernier, nous pouvons sans autre commencer son installation. Une fois cette dernière terminé, il est nécessaire de créer un compte pour se connecter sur l'interface web.

Nous devons ensuite ajouter le/s serveurs pour les monitorer. Pour ajouter un serveur, nous devons nous rendre dans l'ongtet "Devices" puis "Add new device".

Lien de la documentation officiel : [https://community.spiceworks.com/support/network-monitor/docs/setup](https://community.spiceworks.com/support/network-monitor/docs/setup)

L'installation est très simple, il suffit simplement d'attendre que l'executable se soit bien installé. Lorsqu'on ajout des serveurs, les sondes sont automatiquement déployés et configurés. Ce point est un peu dommage, car nous avons pas forcément le controle total. On ne peut seulement modifier les sondes actuelles ou en rajouter via des catégories prédéfinies.

Voici l'interface de spiceworks : 

![](.gitbook/assets/image%20%2812%29.png)

![](.gitbook/assets/image%20%284%29.png)



