# Modèle de Classification de Spam avec TensorFlow

## Introduction

Ce code est un exemple d'un modèle de classification de spam utilisant TensorFlow, une bibliothèque de deep learning. Le modèle est formé pour prédire si un message texte est du spam ou non en se basant sur le texte du message. Le code comprend le prétraitement des données, la création du modèle, la formation du modèle et la visualisation des performances.

## Prérequis

Assurez-vous d'avoir installé les bibliothèques Python suivantes avant d'exécuter le code :

- `tensorflow`
- `pandas`
- `numpy`
- `matplotlib`
- `spacy`
- `en_core_web_sm` (un modèle spaCy en anglais)
- `scikit-learn`

Vous pouvez les installer en utilisant la commande suivante :

```python
!pip install tensorflow pandas numpy matplotlib spacy scikit-learn
```

## Chargement du Dataset

Le code commence par charger un jeu de données qui contient des messages texte étiquetés comme spam ou non-spam.

## Exploration des Données

Le code effectue une analyse exploratoire des données en affichant des statistiques de base telles que la forme du jeu de données, les cinq premières lignes, des statistiques de base et le pourcentage de valeurs manquantes.

## Prétraitement des Données

Le prétraitement des données comprend les étapes suivantes :

- Nettoyage des messages texte en supprimant les caractères non alphanumériques et en convertissant le texte en minuscules.
- Suppression des mots vides (stop words) et lemmatisation des mots restants.
- Encodage des messages texte en utilisant un Tokenizer de TensorFlow.
- Remplissage des séquences pour qu'elles aient la même longueur.

## Séparation des Données d'Entraînement et de Validation

Les données sont divisées en un ensemble d'entraînement et un ensemble de validation pour évaluer les performances du modèle.

## Création du Modèle

Le modèle est un modèle de classification textuelle avec une couche d'embedding, une couche de Global Average Pooling, une couche dense et une couche de prédiction.

## Entraînement du Modèle

Le modèle est entraîné sur les données d'entraînement avec l'optimiseur Adam et la fonction de perte binaire.

## Visualisation des Performances

Des graphiques sont générés pour visualiser les performances du modèle, y compris la perte et l'exactitude au fil des époques.

## Conclusion

Ce code présente un exemple de création d'un modèle de classification de spam en utilisant TensorFlow. Vous pouvez personnaliser ce modèle en modifiant les hyperparamètres, en ajoutant des couches ou en ajustant d'autres aspects du modèle pour obtenir de meilleures performances.
