# Rapport sur le TP1 de Traitement du Langage Naturel

## Introduction

Ce rapport présente les résultats et les méthodes utilisées dans le cadre du premier TP de Traitement du Langage Naturel (NL). L'objectif principal était de nettoyer et d'analyser un ensemble de données textuelles.

## A. Nettoyage et Prétraitement du Texte

1. **Suppression des mots vides** : Utilisation de la liste des mots vides de NLTK pour éliminer les mots courants qui n'apportent pas de signification.
2. **Détection et traduction des langues** : Détermination de la langue de chaque phrase et traduction dans la langue la plus fréquente.
3. **Gestion des homoglyphes et des caractères spéciaux** : Normalisation des caractères spéciaux et suppression des caractères non désirés.
4. **Suppression des mots répétés et des espaces inutiles** : Utilisation d'expressions régulières pour remplacer les mots dupliqués et nettoyer les espaces.

## B. Segmentation du Texte

1. **Segmentation basée sur les espaces et la ponctuation** : Tokenisation des phrases en utilisant `word_tokenize`.
2. **Segmentation basée sur des règles** : Définition de règles pour gérer les contractions et les mots informels.
3. **Tokenisation en sous-mots** : Utilisation de la tokenisation WordPiece pour améliorer la gestion des mots inconnus.

## C. Reconnaissance d'Entités Nommées (NER) et Étiquetage POS

1. **Reconnaissance d'entités nommées** : Extraction des entités nommées à l'aide du modèle `en_core_web_lg` de spaCy.
2. **Étiquetage des parties du discours** : Application de l'étiquetage POS pour identifier la catégorie grammaticale de chaque mot.

## D. Lemmatisation et Stemming

1. **Stemming** : Réduction des mots à leur forme racine à l'aide de `SnowballStemmer`.
2. **Lemmatisation** : Conversion des mots à leur forme de dictionnaire en préservant le sens à l'aide de `WordNetLemmatizer`.

## E. Analyse de Fréquence et Analyse de Sentiment

1. **Compte des mots par auteur** : Utilisation de `CountVectorizer` pour compter les occurrences de mots dans les textes de chaque auteur.
2. **Visualisation des mots les plus utilisés** : Génération de WordClouds pour visualiser les mots les plus fréquents.
3. **Analyse de sentiment des mots** : Mise en œuvre d'un analyseur de sentiment pour classer les mots comme positifs ou négatifs.

## Conclusion

Ce TP a permis d'explorer diverses techniques de prétraitement et d'analyse de texte, fournissant des résultats significatifs sur les données textuelles.
