# Prérequis clients

Prérequis pour les différents clients où les sondes seront configurés..

Schéma infra : 

![](.gitbook/assets/image%20%2811%29.png)

#### OS minimum :

RDP doit être actif pour les OS sous Windows

* Windows 2000 Professional
* Windows 2000 Server
* Windows XP Professional
* Windows Vista
* Windows 7
* Windows 8
* Windows 10
* Windows 2003 Server
* Windows 2008 Server
* Macintosh OS X - **SSH must be enabled**
* Linux/Unix - **SSH must be enabled**

#### Ports qui doivent être ouvert sur les clients :

* Port 161 \(tcp\) SNMP utilisé pour les équipements réseaux
* Port 135 \(tcp\) WMI utilisé pour les serveurs Windows
* ICMP PING utilisé pour un double check si l'host est offline

#### Prérequis spec : 

Aucun agent n'est installés avec Spiceworks, les clients doivent supporter les protocoles WMI, SSH et ICMP pour pouvoir récupérer les informations nécessaires. 







