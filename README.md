# vino

👉 This project is based on a template provided by Johnathan Martel and extended by our team for the Web 2 course.

Projet en cours de développement par les étudiants des groupes de Projet Web 2.

Démo : https://jmartel.webdev.cmaisonneuve.qc.ca/n61/vino/
## Fonctionnalités
Dans l'état de chose, 3 pages sont disponibles.
### Accueil
La page d'accueil affiche les bouteilles de vin qui sont dans le cellier. 
### Ajouter une bouteille
Formulaire qui permet d'ajouter des bouteilles dans le cellier. Le formulaire possède une boite "autocomplete" qui pige dans la base de donnée, les bouteille du catalogue SAQ.
### Importation des bouteilles (BASE_URL/updateSAQ.php)
Script PHP qui permet d'aller récupérer des données du site de la SAQ (pour des fins pédagogiques seulement). Il utilise une classe utilitaire de fonctions d'importation du catalogue de produit de la SAQ. Deux variables sont à définir pour faire l'importation, l'index de la page du catalogue du site Web ($page) et le nombre d'élément à importer ($nombreProduit = 24, 28, 96). L'importation peut être très longue et générer beaucoup d'erreur. Mieux vaut limiter le nombre de bouteilles importées afin d'être efficace dans le développement.

## Installation
### Configuration de la base de données et des définitions (define)
- Renommer dataconf.model.php en dataconf.php 
- Mettre la valeur de la constante BASEURL (main.js)
- Mettre les informations de connexion de la DB dans dataconf.php
- Déployer la base de données qui se trouve dans /data/
- Transférer les fichiers par FTP
- Tester

Bingo.
