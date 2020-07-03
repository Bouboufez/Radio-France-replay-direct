# franceinfo replay
#### version 2.0 alpha 2
franceinfo replay est un petit projet codé sous forme d'une page web pour accéder au replay ou au direct de franceinfo fourni par Radio France directement dans un navigateur.

La page est légère, optimisée pour les appareils mobiles et dispose d'un dark theme.

## Téléchagement

Télécharger la dernière version [ici](https://github.com/Bouboufez/franceinfo-replay/releases).

Ouvrir le fichier html à l'aide d'un navigateur récent et à jour (évitez Internet Explorer).

## Fonctionnalités

Liste des différentes fonctionnalités du projet, et conseils d'utilisations

### Replay

Vous pouvez choisir la date et l'heure à laquelle vous souhaitez revenir pour écouter le replay.

Cliquez sur l'un des jours (aujourd'hui par défaut).

Pour l'heure, entrez une valeur valide (nombre compris entre 0 et 23 ou 59 selon le champ, entier...). Un champ non rempli est compté comme 0 (ce qui permet de ne pas avoir besoin d'insérer les secondes quand on veut aller sur une heure pile par exemple).

### Direct
Il existe également un bouton qui permet directement de lancer la lecture du direct.

### Options avancées
Le menu "options avancées" peut être déplié pour accéder à davantage de réglages.
* Retard du flux : par défaut le flux fourni par Radio France a un retard de 15 secondes, c'est donc la valeur par défaut. Mais vous pouvez changer cette valeur si vous le souhaitez
* Qualité du flux : vous pouvez choisir la qualité du flux que vous souhaitez

Nom | Qualité
------------ | -------------
Auto (par défaut) | Sélectionne automatiquement la qualité selon votre vitesse et type de connexion
Haute | 192 kbps
Standard | 96 kbps
Basse | 32 kbps

### Lecteur
Une fois votre choix (replay ou direct) fait et les paramètres saisis s'ouvre le lecteur.

Ce lecteur peut être mis en pause (le flux est rechargé lors de l'appui sur play), muté, et le volume peut être ajusté.
Des boutons sont présents pour faire une avance ou un recul de 10, 20 ou 30 secondes dans le flux.
Il est également possible d'arrêter la lecture pour reparamétrer son replay.

## Info : objectifs de la version 2.0
Cet été, une version 2.0 du projet devrait voir le jour.

Les changements prévus dans cette nouvelle version sont :
* La page couvrira l'ensemble des antennes de Radio France, et non plus seulement franceinfo. Le thème graphique sera adapté en conséquence
* Il sera possible de passer des arguments directement dans l'URL de la page (de la façon `domaine.com/page.html?argument=valeur` pour gagner du temps. Par exemple, si vous n'écoutez que le direct de franceinfo, vous pourrez mettre en favori l'url modifiée pour accéder directement au replay de franceinfo.
* Diverses améliorations à suivre prochainement

Le développement de la v1 s'arrêtera mais elle sera toujours téléchargeable, et même mise à jour de temps en temps si besoin pour corriger des bugs ou réaliser quelques changements mineurs.

## Remerciements et crédits
La page utilise le lecteur video.js pour lire le flux fourni par Radio France.

franceinfo est un radio de Radio France, tous les droits sur le contenu lu par cette page leur revient. Tous les contenus (images, sons, polices), proviennent directement des serveurs de Radio France et de France.tv. La page ne peut pas être exécutée hors connexion.

Projet initié, créé et maintenu par Bouboufez depuis mai 2020.
