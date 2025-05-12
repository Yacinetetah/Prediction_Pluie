# Prédiction des Précipitations à partir de Données Météorologiques

## Description

Ce projet de science des données vise à construire un modèle prédictif capable d'anticiper les événements de précipitations (pluie) en se basant sur des données météorologiques historiques. L'analyse explore les tendances, gère les défis courants des données météorologiques (valeurs manquantes, séries temporelles) et s'attaque spécifiquement au déséquilibre inhérent entre les jours de pluie et les jours sans pluie.

## Données

Les données utilisées proviennent de relevés météorologiques historiques, incluant diverses variables (température, humidité, vent, pression) 

## Méthodologie

L'approche suit plusieurs étapes clés :

1.  **Chargement et Prétraitement des Données :** Gestion des valeurs manquantes, nettoyage, transformation des features et préparation des données pour l'analyse et la modélisation. Un accent particulier est mis sur la gestion du **déséquilibre de classes** (jours de pluie vs jours sans pluie).
2.  **Analyse Exploratoire et Visualisation :** Comprendre les données, identifier les tendances et visualiser les relations entre les variables.
3.  **Modélisation :** Développement et entraînement d'un modèle de **Deep Learning**, basé sur un réseau de neurones **LSTM** (Long Short-Term Memory), particulièrement adapté aux données séquentielles comme les séries temporelles météorologiques.
4.  **Évaluation :** Évaluation rigoureuse de la performance du modèle en utilisant des métriques adaptées aux problèmes de classification déséquilibrés (Accuracy, Précision, Recall, F1-score).

## Résultats Clés

* Le modèle **LSTM** a démontré une **Accuracy globale de 0.98**, indiquant une très bonne capacité à prédire correctement la majorité des cas.
* Malgré le fort déséquilibre, le modèle montre une capacité prometteuse à détecter la classe minoritaire (précipitations), avec un **F1-score de 0.67** pour la classe "pluie", indiquant un bon équilibre entre précision et rappel pour ces événements moins fréquents.
* L'analyse a permis de mettre en évidence l'importance de la qualité des données et de la gestion du déséquilibre pour ce type de prédiction.

## Technologies et Librairies Utilisées

* **Langage :** Python
* **Librairies de Data Science :** Pandas, NumPy
* **Visualisation :** Matplotlib, Seaborn
* **Machine Learning & Deep Learning :** Scikit-learn, TensorFlow, Keras
* **Gestion du Déséquilibre :** Imbalanced-learn

## Instructions d'Utilisation

1.  **Cloner le dépôt :**
   
2.  **Installer les dépendances :** Assure-toi d'avoir Python 3 installé, puis installe les librairies listées ci-dessus. L'utilisation d'un environnement virtuel est recommandée.
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn tensorflow keras imbalanced-learn # ou utilise un fichier requirements.txt si tu en as un
    ```
3.  **Exécuter l'analyse :** Ouvre et exécute le notebook Jupyter (`IBI .ipynb`) pas à pas dans un environnement Jupyter . Le notebook contient tout le code d'analyse, de modélisation et d'évaluation.

## Auteurs
* TETAH Yacine
* Zabour Sofia
* Kireche Kader
* El Khalil Zenasni

