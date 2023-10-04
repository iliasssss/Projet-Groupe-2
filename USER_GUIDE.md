# Les principales fonctionnalités de KeePass

A présent KeePass est pret à stocker vos mots de passe, mais en priorité nous allons créer votre base de données.

## **Préparer la base de données**

Dérouler le menu Fichier et choisir Nouveau, puis cliquer sur OK dans la boîte de dialogue qui apparaît et confirme la création d'une nouvelle base de données.

![Img1](https://img-19.commentcamarche.net/KjuMxn8EQHq3_uJtX9jPvoyWV5Y=/450x/smart/caf5ddbfdeeb47759e11c15726adf22f/ccmcms-commentcamarche/24056228.png)

Indiquer le dossier dans lequel le fichier .kdbx sera stocké.

![img2](https://img-19.commentcamarche.net/bm1HrE1KJuHiJJSRdoyEuTQuPl4=/450x/smart/70b7dfd734164f63a9828a38b97c145e/ccmcms-commentcamarche/24056242.png)

Il faut maintenant définir le **MasterPASSWORD** qui permet d'accéder à la plateforme qui mémorise tous les mots de passe, il doit être à la fois complexe mais aussi suffisamment simple à retenir.

Pour créer un mot de passe solide nous utiliserons une passphrase :

***(exemple : le Groupe 2 protège vos données personnelles depuis 2023 = lG2pvdpd2023)***

![img3](https://img-19.commentcamarche.net/YtdHVYmP0IX6Ce6bWNi4cjtE0dc=/450x/smart/19b5e6e917ec4e98bb5d26efb9352eeb/ccmcms-commentcamarche/24056267.png)

Cocher la case " Afficher les options de l'Expert", vous aurez la possibilité d'amplifier la securité de la Database en ajoutant "un fichier Clé" en cochant celle-ci et en cliquanr sur "create"

- le fichier clé est un fichier qui contient un clé chiffrée. il ne doit en aucun être modifié sinon vous ne pourriez plus avoir accès à la Database. Cette clè permet d'effectuer une authentification à 2 facteurs (elle meme et le Master Password) pour plus de securité.

![imgage 10](https://github.com/michaelc31/Projet-image/blob/main/Sans%20titre0.png?raw=true)

Sur la page de la creation de la clé, le logiciel vous propose de créer un nouveau fichier clé (avec clé aléatoire) sous 2 formats :

- version 2.0 : nouvelle version du logiciel (version compatible avec KEEPASS2)

- version 1.0 : ancienne version du logiciel (compatible avec les anciennes versions de Keepass et les versions portable) : "Pas utile dans notre cas."

![img](https://github.com/michaelc31/Projet-image/blob/main/Sans%20titre1.png?raw=true)

Sélectionner obligatoirement le premier choix de format de  la clé : "2.0 (recommended), vous arriverez sur une nouvelle fenetre permettant la creation de la clé de 2 manières :

- A la souris : deplacer votre curseur sur le carré de gauche de maniere aléatoire jusqu'a générer une clé de securité suffissament forte.

- Au clavier : Entrer de maniere aléatoire des chaines de caractères afin de générer la clé souhaitée.

![img](https://github.com/michaelc31/Projet-image/blob/main/Sans%20titre2.png?raw=true)

Une fois la nouvelle fenetre affichée, donner un nom à la base de données, puis à sa description si souhaité.

![img4](https://img-19.commentcamarche.net/wGV-MXzwtxzgqoWBXaKndz6Dnqc=/450x/smart/81e13788566a4a708b6c9ca26aabcdcb/ccmcms-commentcamarche/24056269.png)

Pour se souvenir du mot de passe, KeePass propose d'imprimer un formulaire, de le remplir à la main pour le garder à l'abri.
Cliquer sur Imprimer ou Passer.

![img5](https://img-19.commentcamarche.net/5g1hm0h3LJek_6DcbF8AEdeb_y4=/450x/smart/322a4d0591d341caaae46a82a5e5bfc4/ccmcms-commentcamarche/24056271.png)

## **Ajouter des mots de passe**

La base de données est maintenant prête à accueillir les mots de passe. 

Plusieurs Groupes sont répartis au sein de KeePass : Général, Windows, Réseau, Internet, Courriel et Banque à domicile.

Il est possible de créer de nouveaux groupes personnalisables. Pour mémoriser par exemple les identifiants de votre compte Facebook, sélectionner "Internet" puis dérouler le menu "Entrée" et choisir "Ajouter une entrée" (ou raccourci clavier Ctrl + I).

![img6](https://img-19.commentcamarche.net/HJAmv9VjPBwP14xBY1qHbro8fnE=/450x/smart/368b7883baac4ca3baaabf75421bc427/ccmcms-commentcamarche/24056353.png)

Une fois la fenêtre affichée, indiquer dans "Titre" l'intitulé que vous souhaitez enregistré.

Saisir l'identifiant et le mot de passe utilisé pour accéder au compte qui correspond ainsi que l'URL du site Web.

Cliquer sur OK ou Raccourci Ctrl + S pour enregistrer les modifications.

![img7](https://img-19.commentcamarche.net/uH2mW_cVrIZUKYRZrQuWeCJwp1M=/450x/smart/7a22ba78337e43ed99b06fd1f5216db6/ccmcms-commentcamarche/24056366.png)

## Utiliser les mots de passe enregistrés

Une fois la Database créée et fonctionnelle nous allons vous expliquer comment l'utiliser.

Premierement ouvrir Keepass avec la database contenant vous informations personnelles, une fois celle-ci ouverte, il vous faudra d'abord rechercher l'entrée contenant votre mot de passe.

Pour cela, faites `Ctrl+F` ou cliquer sur l'onglet "Find" puis "Find"

![img8](https://github.com/michaelc31/Projet-image/blob/main/Userguid%201.png?raw=true)

Dans le cadre à coté de "Find what" entrer simplement le nom recherché (site web, nom d'utilisateur ...)

la recherche vous affichera toutes les entrées ayant le nom de recherche dans ses informations.

![img9](https://github.com/michaelc31/Projet-image/blob/main/Userguid%20.png?raw=true)

Quand vous avez votre entrée, il suffit simplement d'effectuer un clic droit dessus puis aller sur URL(s) > Open with ... et l'ouvrir avec votre navigateur.

![img10](https://github.com/michaelc31/Projet-image/blob/main/Userguid%203.png?raw=true)

le navigateur internet s'ouvre sur le site associé a la clé,

pour une saisie automatique : il vous suffit de mettre le curseur sur le login et de revenir sur Keepass et d'effectuer un `Ctrl+V` afin que Keepass saisisse automatiquement votre nom d'utilisteur et votre mot de passe .

pour une recuperation de mot de passe : si vous voulez juste afficher votre mot de passe, clic droit sur l'entrée,     edit, et vous aurez accès à l'ensemble des informations de l'entrée.

![img12](https://github.com/michaelc31/Projet-image/blob/main/Suite1.png?raw=true)

Vous pourrez afficher le mot de passe en cliquant sur `...` a coté du mot de passe.

![img13](https://github.com/michaelc31/Projet-image/blob/main/Suite2.png?raw=true)

Vous pourrez copier le mot de passe en le selectionnant et en faissant clic droit "copier"

![img14](https://github.com/michaelc31/Projet-image/blob/main/Suite3.png?raw=true)


## Récupération d'information sur une Entrée :

Comme vous avez pu voir plus haut en récuperant le mot de passe, nous pouvons récupérer n'importe quelle donnée sur une entrée (ex: login, mot de passe, URL ...), pour cela :

- Clic droit sur l'entrée desirée > selectionner "Edit entry" et vous aurez acceè aux informations de la dite entrée.

![img15](https://github.com/michaelc31/Projet-image/blob/main/Suite4.png?raw=true)

## Réglage Auto-Type pour une saisie automatique reussi :

Pour etre sure que le remplissage automatique fonctionne, il vous sera peu etre demander de modifier la commande executer par l'Auto-Type dans l'entrée

Pour se faire, faites un clique droit sur l'entrée est aller sur "edit entry"

![img16](https://github.com/michaelc31/Projet-image/blob/main/Suite5.png?raw=true)

une fois dans l'entrée aller sur l'onglet "Auto-Type", et cocher la "Override default sequence" qui signifie changer la sequence par defaut et remplacer la sequence par 
l'une des sequence suivante selon le type de connexion au site desirée. 
 
 - la sequence {USERNAME}{TAB}{PASSWORD}{ENTER} : sequence par defaut, sert pour les site ou le login et le mot de passe sont sur la meme pages separer en 2 onglets 
 
 - la sequence {USERNAME}{ENTER}{DELAY 1500}{PASSWORD}{ENTER} sert au site avec une connexion en 2 parti: Parti 1 login chargement de page Parti 2 mot de passe (ex : Amazon ...)
 
 - la sequence {USERNAME}{TAB}{TAB}{PASSWORD}{ENTER} : Sequence utile quand le login et le mot de passe sont sur la meme page mais qu'un onglet separe le login et le mot de passe (ex: laposte) 

![img17](https://github.com/michaelc31/Projet-image/blob/main/Suite6.png?raw=true)

# Problème :

| Probleme | Solution   |
|---|---|
| Vous n'arrivez pas a lancer Keepass  | Vérifier que Keepass est bien installé.   |
| Vous n'arrivez pas a vous connecter a la Database |  Etes vous sûr de votre mot de passe ?  |
|   |  Vérifier le chemin d'accès a la database |
|   | Demander au technicien de verifier l'état du reseau  |
| Vous n'arrivez pas a sauvegarder une modification sur la database | Si la database est en local verifier les droits du fichier  |
|   |  Si la database est sur un serveur demander la verification des droits d'acces au fichier |
| Auto-Type ne fonction pas | Verifier que le curseur soit bien sur le login avant de lancer la commande d'Auto-Type |
|   | Verifier la syntaxe de la sequence d'Auto-Type |

