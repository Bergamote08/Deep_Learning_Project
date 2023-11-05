# Modèle de Classification de Spam avec TensorFlow

## Introduction

Ce projet a été developpé dans le cadre de la certification de Machine learning Engineer de Jedha. Il s'agit de développer un modèle de classification de spam. 
Il se base sur les données fournit par AT&T, une compagnie de télécommunication qui souhaite protéger ses usagers des spams.

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

Ce code présente un exemple de création d'un modèle de classification de spam en utilisant TensorFlow. 

## Auteur
Ce notebook a été créé par Charlotte ALLEN
