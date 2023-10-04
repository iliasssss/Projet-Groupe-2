# <p align =center>Projet-Groupe-2 

 ## <p align =center> [Keepass](https://keepass.info/) </p>

**Keepass Password Safe est un gestionnaire de mots de passe permettant de sauvegarder et sécuriser plusieurs mots de passe en un seul fichier chiffré**

## <p align =center> Besoin Initiaux :

Il nous as était demander de crée une Database sécurisé par "Clé" stocké sur un serveur et utilisable par un client.

Une database sécurise par Cle est une database auquel ont as ajouté lors de la création un fichier clé contenant une clé de cryptage generer aleatoirement permetant la liaison entre la database et le mot de passe maitre.

## <p align =center> Etapes d'installation et de configuration :

Vous trouverez un fichier [Install.md](), qui vous servira d'instruction d'installation etape par etape

vous trouverez un fichier [User_Guid.md], qui vous servira a configurer le logiciel Keepass du début.

## <p align =center> Roles Par semaine.

### Semaine 1 
| NOM | Roles | Description |
| :-- |:----- | :---------- |
| Ilias    | Scrum Master      | Garant de la progression et de l'application de la méthode scrum           |
|  Michael   | Product Owner      |   Garant de la qualité du produit final et représentant du client         |
|  Jérôme  |       |             |  Tests et travail sur présentation         |

### Semaine 2 
| NOM | Roles | Description |
| :-- |:----- | :---------- |
| Ilias    |       |            |
|  Michael   | Scrum Master      |  Garant de la progression et de l'application de la méthode scrum          |
|  Jérôme  |  Product Owner     |  Garant de la qualité du produit final et représentant du client          |

## Choix Techniques:

Pour notre projet Keepass, nous avons besoin d'un client et d'un serveur. Notre équipe à choisit de prendre un windows 10 et un windows 2022 serveur ainsi que le logiciel Keepass2 "version2.54" qui est au jour de la documentation la derniere mise a jour de Keepass.

Pour pouvoir acceder a la database sur le client depuis le serveur, nous avons besoin que nous machines soit sur le meme reseaux, la database sera stocké sur un fichier partager. 

## Les difficultées rencontrées
Partage de dossiers/fichiers entre VM impossible 
Droit d'accès de fichier impossible à la database sur le serveur
Problème avec le réseau 

## Les Solutions 

.
.
Faire la liaison entre le réseau NAT et réseau interne
## Les tests réalisés
