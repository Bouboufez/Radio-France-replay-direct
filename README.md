# franceinfo replay
#### version 2.0 alpha 3
franceinfo replay est un petit projet codé sous forme d'une page web pour accéder au replay ou au direct des différentes antennes de Radio France en lisant le flux qu'ils fournissent directement dans un navigateur.

La page est légère, optimisée pour les appareils mobiles et dispose d'un dark theme.

## Version Alpha
**Cette version est une version de développement instable et pas encore aboutie. De nombreuses fonctionnalités sont manquantes ou ne fonctionnent pas correctement.**

## Téléchagement

Télécharger la dernière version alpha ou la dernière version stable [ici](https://github.com/Bouboufez/franceinfo-replay/releases).

Ouvrir le fichier html à l'aide d'un navigateur récent et à jour (évitez Internet Explorer).

## Fonctionnalités
- [ ] A mettre à jour pour la version 2.0

## Etat du projet 2.0
- [x] Ajout du choix de la station et des différents flux correspondants
- [x] Passage à la bibliothèque hls.js pour remplacer video.js pour assurer une meilleure compatibilité
- [x] Retrait de la possibilité de choisir le flux hifi pour les antennes qui n'en disposent pas
- [x] Retrait de la possibilité de choisir le replay pour les flux qui n'en disposent pas (notamment les fipettes semblent ne pas disposer de cette fonctionnalité, à vérifier
- [x] Ajout du bouton direct vidéo pour les radios qui en disposent
- [ ] Ajout d'un deuxième bouton sous le player : "écouter une autre radio"
- [ ] Ajout du support des arguments dans l'URL
- [x] Adaptation du CSS à la charte graphique de Radio France
- [x] Passage de toutes les images en vectoriel/pur CSS
- [x] Adaptation du dark theme au nouveau CSS
- [x] Changement du favicon et du titre de la page qui s"adapte selon le contenu en cours de lecture
- [ ] Ajouter davantage d'animations ? (la charte de RF recommande l'utilisation d'animations douces pour faire apparaître ou disparaître des éléments, afin de permettre une meilleure compréhension du contenu)
- [ ] Tester et s'assurer de la compatibilité de la page sur mobile, et sur différents navigateurs, y compris des navigateurs plus anciens, dans le but de créer un tableau de compatibilité

## Remerciements et crédits
La page utilise la bibliothèque hls.js pour lire les flux fournis par Radio France.

France Inter, franceinfo, France Bleu, France Culture, France Musique, FIP et Mouv' ainsi que leurs locales et webradios thématiques sont des radios de Radio France, tous les droits sur le contenu lu par cette page leur revient. Tous les contenus (images, sons, polices), proviennent directement des serveurs de Radio France et de France.tv. La page ne peut pas être exécutée hors connexion.

Projet initié, créé et maintenu par Bouboufez depuis mai 2020. Version 2.0 développée depuis juillet 2020.
Le projet n'est en aucuh cas lié ou géré par Radio France.
