# Projet de machine learning avec dashboard interactif et API

Ce projet de machine learning comprend un dashboard interactif développé avec **streamlit** et une API déployée sur **heroku**. L'objectif de ce projet est de fournir des prédictions basées sur un modèle de machine learning entraîné.

Ce projet est inspiré de la compétition **kaggle** :    
https://www.kaggle.com/competitions/home-credit-default-risk/

## Partie machine learning
Cette partie contient principalement le notebook de preprocessing et de modélisation ainsi que tous les fichiers qui seront utilisés dans la seconde partie (API et Dashboard)

## Fonctionnalités

- Dashboard interactif basé sur **streamlit**.
- API (**FLASK**) déployée sur **heroku** pour recevoir des requêtes GET et renvoyer des prédictions.
- Modèle de machine learning pré-entraîné utilisé pour les prédictions.

## Structure du projet

Le projet est organisé comme suit :

- dasboard (streamlit)
    -  `streamlit_App.py`: fichier principal pour le dashboard interactif développé avec streamlit.
    -  `dictionnaire.pickle`: permet d'inverser label-encoder et récupérer les noms des classes de chaque variable.
    -  `requirements.txt`: fichier listant les dépendances python requises pour exécuter le projet.

- les autres fichiers (API)
   - `api.py`: fichier contenant le code pour l'API déployée sur heroku.
   - `requirements.txt`: fichier listant les dépendances Python requises pour exécuter le projet.

## Modèle de machine learning

Le détail de la partie machine learning se trouve sur le repo : 
https://github.com/Florian-BOUDON/Scoring_Bancaire_Machine_Learning
- Script evdently permettant d'obtenir les pages html du data drift
- ML-flow 
- Tests unitaires
- Pipeline du meilleur modèle


## Les grandes étapes

1. **Collecte des données** : merging des tables.
2. **Exploration des données** : analyse exploratoire des données pour comprendre leur structure, leurs caractéristiques et effectuer des pré-traitements si nécessaire.
3. **Entraînement du modèle** : sélection d'un algorithme de machine learning, division des données en ensembles d'entraînement et de test, entraînement du modèle sur les données d'entraînement.
4. **Évaluation du modèle** : évaluation des performances du modèle à l'aide de métriques appropriées et ajustement des hyperparamètres création d'une fonction de perte.
5. **Développement du dashboard** : création d'un dashboard interactif.
6. **Déploiement de l'API** : déploiement de l'API sur heroku pour permettre l'accès aux prédictions du modèle via des requêtes GET.

## Prérequis

Avant d'exécuter le projet, assurez-vous d'avoir installé les dépendances suivantes :

- Python 3.x
- Les bibliothèques python spécifiées dans le fichier `requirements.txt`


## Utilisation streamlit

Afficher le dashboard streamlit : https://dashboard-v3.streamlit.app/


## Utilisation heroku

Afficher le dashboard streamlit : https://api-scoring-194928115115.herokuapp.com/
- point d'API GET :https://api-scoring-194928115115.herokuapp.com/proba
- point d'API POST :https://api-scoring-194928115115.herokuapp.com/predict    

*********
Ce projet fait partie de la formation data-scientist de CentraleSupélec & Openclassrooms (certificat bac+5).
  
