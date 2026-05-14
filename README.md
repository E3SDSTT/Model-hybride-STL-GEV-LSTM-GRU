# Model-hybride-STL-GEV-LSTM-GRU
Model hybride STL-GEV-LSTM et GRU pour la prédiction des débits hydrologique dans le bassin du Mono en utilisant les paramètres univariés et multivariés tels que les données climatique

Ce dépôt contient l'implémentation complète d'une approche hybride combinant décomposition statistique, théorie des valeurs extrêmes et Deep Learning pour la prévision des crues dans le bassin du Mono (Togo).

## Présentation du Projet
L'objectif est de prévoir les débits mensuels paroxystiques à l'aide d'une méthodologie en plusieurs étapes :
*   **Décomposition STL** : Isolation de la composante résiduelle des chroniques de débits.
*   **Modélisation GEV** : Application de la loi des valeurs extrêmes sur les résidus.
*   **Transformation CDF** : Projection dans un espace probabiliste [0, 1] pour stabiliser l'apprentissage.
*   **Deep Learning** : Comparaison des modèles Séquentiel, LSTM et GRU en configurations univariée et multivariée.

## 📊 Données
*   **Hydrologie (1952-2023)** : Débits des stations de Dotaicopé, Corrékopé et Tététou.
*   **Météorologie (1981-2023)** : Précipitations, températures et humidité issues de **NASA POWER**.

## 🛠️ Installation
Pour exécuter ce notebook, installez les dépendances suivantes :
```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels tensorflow scikit-learn
