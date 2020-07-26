# Radio France • Replay et direct

#### Version 2.0.1 (26/07/2020)

Petit projet permettant d'écouter l'ensemble des antennes radios de Radio France, en direct et en replay pour les flux qui le supportent, directement dans un navigateur.

La page est légère, optimisée pour les appareils mobiles et dispose d'un dark theme.

## Téléchargement
Vous pouvez télécharger la dernière version du projet [à cette adresse](https://github.com/Bouboufez/franceinfo-replay/releases).
<br>Il vous suffit ensuite uniquement d'ouvrir le fichier dans votre navigateur favori.

### Compatibilité
Le projet est compatibile avec tous les navigateurs récents (Firefox, Chrome, Edge...) et relativement à jour, y compris Internet Explorer 11 sur Windows 8.1 et 10 **uniquement**.
<br>Il fonctionne sur ordinateur comme sur mobiles et tablettes.

## Utilisation

### Prise en main

#### Choix de la station
Il vous faut tout d'abord chosir dans la liste la radio que vous souhaitez écouter, puis si besoin dans une seconde liste sélectionner la locale ou la webradio de votre choix.
<br> Une fois ce choix fait, vous pouvez choisir d'écouter le direct ou le replay en spécifiant des options.

#### Replay
Si vous choisissez d'écouter la radio en replay, vous pouvez entrer la date et l'heure à laquelle vous souhaitez revenir pour écouter le replay.

Cliquez sur l'un des jours (aujourd'hui par défaut). Il est possible de remonter à J-2 au maximum.
<br>Pour l'heure, entrez une valeur valide (nombre compris entre 0 et 23 ou 59 selon le champ, entier...). Un champ non rempli est compté comme 0 (ce qui permet de ne pas avoir besoin d'insérer les secondes quand on veut aller sur une heure pile par exemple).

Vous pouvez ensuite lancer la lecture à l'aide du bouton "Écouter le replay".

**__Note :__** La fonction replay n'est pas disponible pour toutes les antennes de FIP, ainsi que sur toutes les webradios.

#### Direct
De la même façon, vous pouvez trouver en dessous un bouton qui permet de lancer la lecture en direct.
<br>Par ailleurs, sur les antennes de France Inter, franceinfo: et Mouv' (national), vous pouvez lancer le direct vidéo *(lien vers Dailymotion)*.

### Lecteur audio
Une fois le direct ou le replay sélectionné, la lecture se lance et le lecteur audio apparaît.

Ce lecteur peut être mis en pause (le flux est rechargé lors de l'appui sur play à l'endroit où vous l'avez arrêté), muté, et le volume peut être ajusté. 
<br>Pour savoir où vous en êtes, l'heure de diffusion s'affiche (précision de plus ou moins 5 secondes lors du replay).
<br>Des boutons sont présents pour faire une avance ou un recul de 10, 20 ou 30 secondes dans le flux. 
<br>Il est également possible de choisir une autre heure ou une autre station (attention : cela ferme le lecteur, fait réapparaître le formulaire et retire tous les arguments dans l'URL).

### Fonctions avancées

#### Dark theme
Le projet dispose d'un light theme (par défaut) et d'un dark theme pour permettre le meilleur affichage possible.
<br>Le choix du theme est automatiquement fait par votre navigateur selon vos préférences système.

#### Options avancées
En bas du formulaire, le bouton "options avancées" permet de définir des options supplémentaires.

##### Retard du flux
Par défaut le flux fourni par Radio France a un retard de 15 secondes, c'est donc la valeur par défaut. Mais vous pouvez changer cette valeur si vous le souhaitez, de 0 à 60 secondes.

##### Qualité du flux
Vous pouvez choisir la qualité du flux lu dans le lecteur audio.
<br>**Pour les flux nationaux :** (la majorité des flux)

Nom | Qualité
------------ | -------------
Auto (par défaut) | Flux adaptatif : sélectionne automatiquement la qualité selon votre vitesse et type de connexion
Basse | 32 kbps
Standard | 96 kbps
Haute | 192 kbps

**Pour les flux régionaux :** (France Bleu (sauf France Bleu Paris) et antennes régionales de FIP)

Nom | Qualité
------------ | -------------
Auto (par défaut) | Flux adaptatif : sélectionne automatiquement la qualité selon votre vitesse et type de connexion
Basse | 32 kbps
Standard | 128 kbps

#### Arguments URL
Il est désormais possible de passer des arguments directement dans l'URL de la page (de la forme `https://domaine.fr/RF replay direct.html?PARAM1=VALEUR1&PARAM2=VALEUR2`).
<br>**Liste des paramètres acceptés :**

Paramètre | Valeurs acceptées | Utilité | Exemple
------------ | ------------- | ------------- | -------------
`radio` | Noms des stations tels qu'utilisés dans les liens des flux fournis par Radio France | Permet de sélectionner une station | `RF replay direct.html?radio=franceinter`
`h` | Nombre entier entre 0 et 23 | Permet de choisir l'heure (replay) | `RF replay direct.html?h=20`
`m` | Nombre entier entre 0 et 59 | Permet de choisir les minutes (replay) | `RF replay direct.html?m=30`
`s` | Nombre entier entre 0 et 59 | Permet de choisir les secondes (replay) | `RF replay direct.html?s=59`
`j` | Nombre entier entre 0 et 2 | Nombre de jours à remonter (0 = aujourd'hui, 1 = hier, 2 = avant-hier) | `RF replay direct.html?j=2`
`delay` | Nombre entier entre 0 et 60 | Valeur du retard du flux | `RF replay direct.html?delay=15`
`flux` | `auto` (Auto), `lofi` (Basse), `midfi` (standard), `hifi` (haute si disponible) | Qualité du flux | `RF replay direct.html?flux=hifi`

##### Astuce
Si vous avez l'habitude d'écouter une certaine station (par exemple France Culture), mettez en favori le lien `RF replay direct.html?radio=franceculture` pour ne pas avoir à sélectionner la même station à chaque ouverture de la page !

## Remerciements et crédits
La page utilise la bibliothèque hls.js pour lire les flux fournis par Radio France.

France Inter, franceinfo, France Bleu, France Culture, France Musique, FIP et Mouv' ainsi que leurs locales et webradios thématiques sont des radios de Radio France, tous les droits sur le contenu lu par cette page leur revient. Tous les contenus (images, sons, polices), proviennent directement des serveurs de Radio France et de France.tv. La page ne peut pas être exécutée hors connexion.

Projet initié, créé et maintenu par Bouboufez depuis mai 2020. Le projet n'est en aucun cas lié ou géré par Radio France.
