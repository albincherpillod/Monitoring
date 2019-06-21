# FileServer-WindowsCore

Pour s'y connecter, il faut utiliser le protocole RDP, en utilisant l'application "mstsc" de Windows.

Une fois la console ouverte, nous allons installer le rôle "File-Services". 

#### Installation service

Il faut tout d'abord passer en powershell, il suffit de tapper "powershell"

![](.gitbook/assets/image%20%283%29.png)

Puis on lance la commande "Install-WindowsFeature File-Services"

![](.gitbook/assets/image%20%2818%29.png)

Le service File Server n'est pas répertorié dans les services accessibles depuis Spiceworks. Du coup, j'ai décidé d'installé le rôle IIS. Le service se nomme : W3SVC

Pour l'installer, il suffit de passer la commande suivante :

```text
Install-WindowsFeature Web-Server
```

![](.gitbook/assets/image%20%2815%29.png)

Une fois le service ajouté dans la liste à monitorer, je l'ai arrêter pour vérifier la remonté d'alerte.

![](.gitbook/assets/image%20%2819%29.png)

![](.gitbook/assets/image%20%2821%29.png)

Nous avons directement l'alerte sur l'interface et également une alerte nous est transmises par email

![](.gitbook/assets/image%20%2817%29.png)

