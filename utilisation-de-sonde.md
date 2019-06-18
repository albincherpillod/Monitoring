# Utilisation de sonde

Pour pouvoir tester l'utilisation d'une sonde, j'ai téléchargé un logiciel qui va va monter le CPU à 100%. 

Le logiciel "CPU Stress MT" a été utilisé et démarré :

![](.gitbook/assets/image%20%287%29.png)

![](.gitbook/assets/image%20%281%29.png)

Un email a également été envoyé par Spiceworks

![](.gitbook/assets/image%20%2810%29.png)

#### Linux

Pour faire un stress du CPU sous Centos, nous devons utiliser la commande : stress

```text
sudo yum install epel-release 
sudo yum install stress
stress-ng --cpu 4 --timeout 60s
```

