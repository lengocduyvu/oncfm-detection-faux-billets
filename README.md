# Détecteur de faux billets

## Description
**ONCFM - Organisation nationale de lutte contre le faux-monnayage** est une organisation publique ayant pour objectif de mettre en place des méthodes d'identification des contrefaçons des billets en euros.
Dans le cadre de cette lutte, nous souhaitons mettre en place un algorithme qui soit capable de différencier automatiquement les vrais des faux billets.

Lorsqu'un billet arrive, nous avons une machine qui consigne l'ensemble de ses caractéristiques géométriques. Au fil de nos années de lutte, nous avons observé des différences de dimensions entre les vrais et les faux billets. Ces différences sont difficilement visibles à l'oeil nu, mais une machine devrait sans problème arriver à les différencier.

Ainsi, il faudrait construire un algorithme qui, à partir des caractéristiques géométriques d'un billet, serait capable de définir si ce dernier est un vrai ou un faux billet.

## Structure du projet
- `data/` :         Contient les jeux de données utilisés pour le projet.
- `notebooks/` :    Contient les notebooks Jupyter utilisés pour l'analyse des données.
- `gfx/` :          Contient les graphiques utilisés.
- `reports/` :      Contient les rapports générés à partir des analyses.

## Première partie : Analyse exploratoire
- Vérification des données
- Analyse descriptive
- Régression linéaire pour compléter les valeurs manquantes
- Analyse des outliers
- Entraînement, test et optimisation des modèles de classification par hyperparamètres
- Sélection du meilleur modèle de classification
- Sauvegarde du modèle entraîné

## Deuxième partie : Application
- Mise en production du modèle de classsification entraîné sur une nouveau jeu de données
- Utilisation d'un pipeline avec transormation des données
- Traitement de la conformité des colonnes
- Traitement des valeurs manquantes par régression linéaire
- Standardisation des données
- Prédiction

## Prérequis
- Python 3.x
- Jupyter Notebook
- Bibliothèques Python : pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels, scipy

## Installation
1. Clonez le dépôt :
    ```bash
    git clone https://github.com/lengocduyvu/oncfm-detection-faux-billets.git
    ```
2. Installez les dépendances :
    ```bash
    pip install -r requirements.txt
    ```

## Utilisation
1. Lancez Jupyter Notebook :
    ```bash
    jupyter notebook
    ```
2. Ouvrez et exécutez les notebooks dans le dossier `notebooks/`.

## Auteur
- Ngoc LE (https://github.com/lengocduyvu)