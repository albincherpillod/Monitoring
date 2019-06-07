# Installation de Spiceworks

Spiceworks est un ....

#### Prérequis Serveur

| SPEC |  |
| :--- | :--- |
| OS | 64-bit Windows - Win Server 2012 R2 |
| CPU | Dual-core CPU |
| RAM | 4GB |
| Disque | At least 50 GB |

#### Dépendance 

Le firmware .NET 4.5 est nécessaire pour l'installation de cette solution.

#### Sécurité

![](.gitbook/assets/image%20%286%29.png)

* 4094 - collector service
* 5555 - Processor service
* 6739 - redis database
* 8005 - app server
* 8009 - app server

#### Mise en place 

Pour l'installation de l'outil de monitoring Spiceworks, nous devons tout d'abord nous connecter en remote sur notre serveur. 

Une fois la connexion établie, nous devons nous rendre sur le site de Spiceworks pour télécharger l'exécutable. Un compte est nécessaire pour le téléchargement.

{% embed url="https://www.spiceworks.com/download/monitor" %}

Suite au téléchargement de ce dernier, nous pouvons sans autre commencer son installation.

Une fois l'installation terminée, le lien web s'ouvre automatiquement. Nous devons ensuite ajouter le/s serveurs pour les monitorer. Pour ajouter un serveur, nous devons nous rendre dans l'ongtet "Devices" puis "Add new device".

Lien de la documentation officiel : [https://community.spiceworks.com/support/network-monitor/docs/setup](https://community.spiceworks.com/support/network-monitor/docs/setup)

Voici l'interface de spiceworks : 

![](.gitbook/assets/image.png)

![](.gitbook/assets/image%20%281%29.png)

