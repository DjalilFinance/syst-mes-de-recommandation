Recommandation Clients


Description

Ce projet implémente un système de recommandation pour personnaliser les offres et produits selon les préférences des clients. Il utilise des modèles de deep learning (DeepRecommender) pour générer des recommandations 

précises à partir de données utilisateur, en intégrant une API pour une utilisation en production.


Structure du projet

DeepRecommender/ : Contient les modèles de deep learning pour le système de recommandation.

data/ : Ensemble de données utilisateur pour entraîner et tester les modèles.

Intro_Recommender.ipynb : Notebook explicatif sur la mise en œuvre du système de recommandation.

api.py : API pour déployer et consommer le système de recommandation.

load_test.py : Script de test de charge pour évaluer les performances de l'API.

parameters.py : Contient les configurations et hyperparamètres du modèle.

utils.py : Fonctions auxiliaires pour le prétraitement des données et l'évaluation des modèles.

Fonctionnalités clés

Modélisation avancée pour les systèmes de recommandation (DeepRecommender).

API REST pour consommer les recommandations en production.

Tests de charge pour garantir la robustesse des services.

Entraînement et évaluation des modèles sur des ensembles de données personnalisés.

Installation

Clonez ce dépôt :



bash

Copier le code

git clone https://github.com/ton_profil/Recommandation_clients.git

cd Recommandation_clients

Installez les dépendances :



bash

Copier le code

pip install -r requirements.txt

Lancez l’application API :


bash

Copier le code

python api.py

Utilisation

API REST :

Envoyez une requête POST pour obtenir des recommandations pour un utilisateur spécifique.

Exemple de requête :



bash

Copier le code

curl -X POST -H "Content-Type: application/json" \

     -d '{"user_id": 123}' http://127.0.0.1:5000/recommend

Notebook :

Utilisez Intro_Recommender.ipynb pour explorer et comprendre le fonctionnement du système de recommandation.

Technologies utilisées

Langages : Python.

Frameworks : Flask (API), TensorFlow/PyTorch (DeepRecommender).

Bibliothèques : NumPy, Pandas, Scikit-learn.

Contributeurs

Salah Bey Abdeldjalil
