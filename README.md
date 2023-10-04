# <p align =center>Projet-Groupe-2 

### <p align =center> [Keepass](https://keepass.info/)
 
**Keepass Password Safe est un gestionnaire de mots de passe permettant de sauvegarder et sécuriser plusieurs mots de passe en un seul fichier chiffré**


## <p align =center> Besoin Initiaux :

Il nous as était demander de crée une Database sécurisé par "Clé" stocké sur un serveur et utilisable par un client.

Une database sécurise par Cle est une database auquel ont as ajouté lors de la création un fichier clé contenant une clé de cryptage generer aleatoirement permetant la liaison entre la database et le mot de passe maitre.


## <p align =center> Etapes d'installation et de configuration :

Vous trouverez un fichier [Install.md](https://github.com/iliasssss/Projet-Groupe-2/blob/main/Install.md), qui vous servira d'instruction d'installation etape par etape

vous trouverez un fichier [User_Guid.md](https://github.com/iliasssss/Projet-Groupe-2/blob/main/USER_GUIDE.md), qui vous servira a configurer le logiciel Keepass du début.


## <p align =center> Roles Par semaine.

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


## <p align =center> Choix Techniques:

Pour notre projet Keepass, nous avons besoin d'un client et d'un serveur. Notre équipe à choisit de prendre un windows 10 et un windows 2022 serveur ainsi que le logiciel Keepass2 "version2.54" qui est au jour de la documentation la derniere mise a jour de Keepass.

Pour pouvoir acceder a la database sur le client depuis le serveur, nous avons besoin que nous machines soit sur le meme reseaux, la database sera stocké sur un fichier partager. 


## <p align =center> Les difficultées rencontrées

Durant nos different test, nous avons etait confronter a different probleme: 

 -  Partage de dossiers/fichiers entre VM impossible : une fois les machines bien configurer au niveau réseaux (adressage et parefeu), le partage de fichier n'etait pas toujours disponible.  
 
 -  Droit d'accès de fichier impossible à la database sur le serveur : une fois la Database sur le serveur, le client se connecte dessus apres modification de la database impossibilité de sauvegarder

 -  Probleme avec AutoType : Selon les sites et leur façon de se connecter l'AutoType marche pas forcément


## <p align =center> Les Solutions 

Pour resoudre les differents problemes rencontrés nous avons effectuer different test se qui nous as permis de trouver les solution suivant aux problemes:
 
 -  Partage de dossiers/fichiers entre VM impossible : l'impossibilité de se connecter au dossier partager venait d'un conflit de carte reseau sur les VM. Après differents test il s'est avéré que les carte reseau devait etre configurer de la maniere suivante pour le client: 1 premiere carte Nat avec connexion a internet et 1 seconde carte interne avec la configuration reseau parametrer dessus. et pour le serveur on est rester sur 1 carte interne.
 
 -  Droit d'accès de fichier impossible à la database sur le serveur : Apres different test il s'est avéré que le souci venez d'un oubli de droits sur l'utilisateur se qui empecher la sauvegarde de la Database.
 
 -  Il faut selon le site faire un reglage dans les commande AutoType pour que celle ci fonctionne et remplacer la ligne {USERNAME}{TAB}{PASSWORD}{ENTER} par {USERNAME}{TAB}{TAB}{PASSWORD}{ENTER} ou {USERNAME}{ENTER}{DELAY=1000}{PASSWORD}{ENTER} 


## <p align =center> Les tests réalisés

Durant les 2 dernieres semaines nous avons realiser les test suivants:

-- Création de VM avec OS Windows10 et Windows22 server

-- Mise en réseaux des VM : configuration IP, verification de comunication avec la commande `Ping`

-- Télechargement du Logiciel Keepass2 et test en local : Création Database classique, création d'entrée, test AutoType, Réglage AutoType.

-- Création et Test de Database Final du Projet : Création d'une Database Securisé par Clé, création d'un User, Création des diverses entrées de la Database

-- Mise en Réseau de la Database : Création du Dossier Partager pour la liaison entre le client et le serveur

-- Test de recuperation de la Database sur le serveur.

-- Utilisation de Keepass en condition réél

-- Test Présentation
