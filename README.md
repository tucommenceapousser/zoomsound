# File Read Zoomsound Python Script

Ce script Python est conçu pour effectuer une opération de lecture de fichier arbitraire (Unauthenticated) sur un plugin WordPress appelé "DZS Zoomsounds" avec la version 6.45. Le script utilise la commande `curl` pour effectuer une requête HTTP sur un site WordPress cible et lire un fichier spécifié.

## Google Dork

Un Google Dork est une requête de recherche spécifique utilisée pour trouver des informations sensibles exposées publiquement sur Internet. Dans ce script, nous utilisons le Google Dork suivant pour rechercher des sites WordPress vulnérables utilisant le plugin DZS Zoomsounds :
```
inurl:/wp-content/plugins/dzs-zoomsounds/
```
Ce dork nous permet de trouver des sites WordPress qui utilisent ce plugin spécifique.

## Utilisation du Script

1. Le script commence par afficher une bannière amusante avec le texte "File Read Zoomsound" en utilisant le module `pyfiglet`.

2. Ensuite, il demande à l'utilisateur de fournir l'URL de l'hôte cible (par exemple, `https://example.com`). Si l'utilisateur appuie simplement sur Entrée, il utilisera l'URL d'exemple par défaut.

3. Le script demande également le chemin du fichier à lire sur le serveur cible. Par défaut, il tente de lire le fichier `../../../../../../../../../../etc/passwd`. Si l'utilisateur appuie sur Entrée, il utilisera cette valeur par défaut.

4. Il exécute ensuite une commande `curl` pour tenter de lire le fichier spécifié sur le serveur WordPress cible.

5. Le script affiche la réponse obtenue avec succès ou les erreurs qui se sont produites lors de la tentative de lecture du fichier.

6. Il demande également à l'utilisateur s'il souhaite enregistrer le contenu dans un fichier `.txt`. Si l'utilisateur accepte, il lui demande de spécifier le nom du fichier de sauvegarde.

7. En fin de compte, le script affiche un message indiquant si le fichier a été enregistré avec succès.

## Exécution du Script

Pour exécuter ce script, assurez-vous d'avoir Python installé sur votre système. Vous devrez également installer les bibliothèques Python requises en utilisant `pip install -r requirements.txt`. Ensuite, vous pouvez exécuter le script en utilisant la commande `python main.py`.

**Note importante :** L'utilisation de ce script pour des activités non autorisées sur des sites Web auxquels vous n'avez pas l'autorisation d'accéder peut être illégale. Assurez-vous d'obtenir l'autorisation du propriétaire du site avant de l'utiliser sur un site en production.

## Auteur

Ce script a été créé par TRHACKNON et est distribué sous licence MIT.