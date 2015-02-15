# twitterproject
récolter et représenter les tweets en temps réel. Pour pouvoir lancer les programme il faut d'abord enregistrer un compte application sur apps.twitter.com pour obtenir les 4 codes d'accès nécéssaires au streaming.
### Dans ce dépôt:

Dans ce dépôt deux programmes qui sont destinés à tourner côté serveur pour récolter les tweets sur un hashtag en temps réel. Le premier script python se contente de les stocker dans une base de données et d'effectuer quelque requêtes de base. le script JS tourne dans un service NodeJS, à l'aide des websockets il "stream" les positions des tweets géolocalisés vers une page htl cliente qui les places sur un fonds de carte en utiliasnt heatmap/leaflet.

### satisfaire les dépendances:
Les deux programmes ont besoins d'un cerain nombre de paquets pour tourner.

- Pour le programme python:

  ```
  sudo pip install tweepy pymongo
  ```
  
  J'ai préparé un petit script pour tout installer il suffit de lancer :
  
  ```
  bash install.sh
  ```
  
- Pour le programme NodeJS:
  
  Il suffit de lancer :

  ````
   sudo npm install
   ````

### Lancer les programmes:

- Lancer le programme Python:
  
  Il faut d'abord renseigner les HashTag que vous voulez suivre. Pour cela éditer le fichier launch.sh et lancer le après en utilisant les deux commandes suivantes:

  ```
  vi launch.sh
  ./launch.sh
  ```
  
  - Lancer le serveur NodeJS:
  
  Il suffit de lancer la commande suivante:
  ```
  node tweet.js
  ```

### Snapshot:
