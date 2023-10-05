# <p align =center> <font color='green'> Projet-Groupe-2 </font> </p> 

### <p align =center> [Keepass](https://keepass.info/)
 
**Keepass Password Safe est un gestionnaire de mots de passe permettant de sauvegarder et sécuriser plusieurs mots de passe dans un seul fichier chiffré**.


## <p align =center> Besoins Initiaux

Demande de base : créer une Database sécurisée par "Clé" stockée sur un serveur et utilisable par un client.

Une database sécurisée par clé est une database à laquelle nous ajoutons, lors de sa création, un fichier clé contenant une clé de cryptage générée aleatoirement. Cela permet la liaison entre la database et le mot de passe maitre.


## <p align =center> Etapes d'installation et de configuration

Vous trouverez un fichier [Install.md](https://github.com/iliasssss/Projet-Groupe-2/blob/main/Install.md), qui vous servira d'instruction d'installation étape par étape

vous trouverez un fichier [USER_GUIDE.md](https://github.com/iliasssss/Projet-Groupe-2/blob/main/USER_GUIDE.md), pour vous aider à configurer le logiciel Keepass pas à pas.


## <p align =center> Rôles par semaine

### Semaine 1 
| NOM | Roles | Description |
| :-- |:----- | :---------- |
| Ilias    | Scrum Master      | Garant de la progression et de l'application de la méthode scrum    |
|  Michael   | Product Owner      |  Garant de la qualité du produit final et représentant du client   |
|  Jérôme  |       |             |  Tests et travail sur présentation   |

### Semaine 2 
| NOM | Roles | Description |
| :-- |:----- | :---------- |
| Ilias    |       |            |
|  Michael   | Scrum Master      |  Garant de la progression et de l'application de la méthode scrum   |
|  Jérôme  |  Product Owner     |  Garant de la qualité du produit final et représentant du client    |


## <p align =center> Choix Techniques

Pour notre projet Keepass, nous avons besoin d'un client et d'un serveur. Notre équipe a choisi de prendre un windows 10 et un windows 2022 serveur ainsi que le logiciel Keepass2 "version2.54" qui est à ce jour (05/10/2023) la dernière version de Keepass.

Pour pouvoir accéder à la database sur le client depuis le serveur, nous avons besoin que nos machines soient sur le même réseau, la database sera stockée sur un fichier partagé. 


## <p align =center> Les difficultés rencontrées

Durant nos différents tests, nous avons eté confronté aux incidents suivants: 

 -  Partage de dossiers/fichiers entre VM impossible : une fois les machines bien configurées au niveau réseau (adressage et parefeu), le partage de fichier n'etait pas toujours disponible.  
 
 -  Droit d'accès de fichier impossible à la database sur le serveur : une fois la Database sur le serveur, le client se connecte dessus apres modification de la database mais il était impossible de la sauvegarder.

 -  Incident avec "AutoType" : selon les sites et leur mode d'authentification "l'AutoType" ne fonctione pas systématiquement.


## <p align =center> Les solutions 

Pour resoudre les differents incidents rencontrés nous avons effectué de nombreux tests pour parvenir aux solutions suivantes :
 
 -  Partage de dossiers/fichiers entre VM impossible : l'impossibilité de se connecter au dossier partagé venait d'un conflit de carte reseau sur les VM. Après differents tests il s'est avéré que les cartes reseaux devaient etre configurées de la maniere suivante pour le client: 1 première carte Nat avec connexion à internet et 1 seconde carte interne avec la configuration réseau parametrer dessus et pour le serveur nous avons activé qu'une seule carte réseau interne (Intnet).
 
 -  Droit d'accès de fichier impossible à la database sur le serveur : après plusieurs vérifications des propriétés réseaux et de partage nous avions omi les droits pour l'utilisateur en mode écriture cequi empechait la sauvegarde de la Database.
 
 -  Il faut selon le site faire un reglage dans les commandes AutoType pour que celle-ci fonctionne et remplace la ligne {USERNAME}{TAB}{PASSWORD}{ENTER} par {USERNAME}{TAB}{TAB}{PASSWORD}{ENTER} ou {USERNAME}{ENTER}{DELAY=1000}{PASSWORD}{ENTER} 


## <p align =center> Les tests réalisés

Durant les 2 dernieres semaines nous avons realisé les tests suivants:

-- Création de VM avec OS Windows10 et Windows22 server.

-- Mise en réseau des VM : configuration IP, vérification de communication avec la commande `Ping`.

-- Téléchargement du Logiciel Keepass2 et test en local : Création Database classique, création d'entrée, test AutoType, Réglage AutoType.

-- Création et Test de Database Final du Projet : création d'une Database sécurisée par Clé, création d'un utilisateur, création des diverses entrées de la Database.

-- Mise en Réseau de la Database : création du dossier partagé pour la liaison entre le client et le serveur.

-- Test de récuperation de la Database sur le serveur.

-- Utilisation de Keepass en condition réélle.

-- Test démonstration pour la présentation.
