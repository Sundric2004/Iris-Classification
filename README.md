# Classification des Iris : Pipeline de Machine Learning Professionnel

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange.svg)](https://scikit-learn.org/)
[![Gradio](https://img.shields.io/badge/UI-Gradio-orange.svg)](https://gradio.app/)

Ce projet présente une approche professionnelle pour la classification des espèces d'Iris. Contrairement à un script classique, il utilise des **Pipelines** pour garantir la robustesse des données et intègre à la fois des méthodes d'apprentissage supervisé et non-supervisé.



##  Objectifs du Projet
L'objectif est de prédire l'espèce d'une fleur d'Iris (*Setosa*, *Versicolor*, ou *Virginica*) à partir de quatre caractéristiques morphologiques : longueur et largeur des sépales et des pétales.

## Fonctionnalités principales

### 1. Analyse Exploratoire des Données (EDA)
- Visualisation des distributions et des corrélations via des graphiques croisés.
- Identification des séparations naturelles entre les classes.

### 2. Pipeline de Classification (Supervisé)
- **Prétraitement** : Normalisation automatique via `StandardScaler`.
- **Modèle** : Utilisation de `RandomForestClassifier` pour sa robustesse et sa gestion des relations non-linéaires.
- **Évaluation** : Analyse par matrice de confusion et rapport de classification (Précision/Recall).



### 3. Analyse Avancée (Non-supervisé)
- **ACP (PCA)** : Réduction de la dimensionnalité de 4D à 2D pour visualiser la structure des données.
- **K-Means Clustering** : Détection automatique des groupes pour comparer les regroupements statistiques aux espèces réelles.



### 4. Interface de Déploiement
- Création d'une application web locale avec **Gradio**.
- Interface avec curseurs (sliders) permettant de tester le modèle en temps réel de manière interactive.

##  Installation

1. **Cloner le projet** :
   ```bash
   git clone [https://github.com/votre-utilisateur/iris-classification-pro.git](https://github.com/votre-utilisateur/iris-classification-pro.git)
   cd iris-classification

2. **Installer les dépendances**

## Utilisation

**Exécution du Notebook**

Ouvrez le fichier Iris_Classifications.ipynb dans Jupyter Notebook ou VS Code.
Toutes les étapes sont documentées, du chargement des données (iris.data) au déploiement de l'interface.
Lancer l'interface de prédiction
Exécutez la dernière cellule du notebook pour lancer Gradio. Vous pourrez alors accéder à l'interface via votre navigateur à l'adresse suivante : http://127.0.0.1:7860.

## Résultats

Le modèle de forêt aléatoire (Random Forest) inclus dans le pipeline permet d'atteindre une précision de 97% à 100% sur le jeu de test. L'utilisation du pipeline garantit qu'aucune donnée de test ne "fuit" dans l'entraînement (Data Leakage), respectant ainsi les standards de l'industrie.
