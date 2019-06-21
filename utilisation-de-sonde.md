# Utilisation de sonde

Pour pouvoir tester l'utilisation d'une sonde, j'ai téléchargé un logiciel qui va va monter le CPU à 100%. 

Le logiciel "CPU Stress MT" a été utilisé et démarré :

![](.gitbook/assets/image%20%2812%29.png)

![](.gitbook/assets/image%20%282%29.png)

Un email a également été envoyé par Spiceworks

![](.gitbook/assets/image%20%2822%29.png)

#### Linux

Pour faire un stress du CPU sous Centos, nous devons utiliser la commande : stress

```text
sudo yum install epel-release 
sudo yum install stress
stress-ng --cpu 4 --timeout 60s
```

#### Serveur Windows Core - Powershell

Pour stresser le CPU d'un serveur Core, nous pouvons utiliser un script powershell. Ce dernier a été récupéré sur ce [lien](http://robvit.com/windows_server/generate-cpu-load-with-powershell/) et enregistrer sur le serveur. Le stress s'est bien effectué et le monitoring a pu détecté la monté de charge.  

![](.gitbook/assets/image%20%288%29.png)

![](.gitbook/assets/image%20%2814%29.png)

