# Projet Big Data – Pig et MapReduce

## Description
Ce projet explore le traitement de grandes quantités de données avec Hadoop, Pig et MapReduce. Il couvre la manipulation de fichiers texte, le calcul de TF-IDF, la transformation de données relationnelles et l’utilisation de fonctions personnalisées (UDF).

## Pig
- Langage : Pig Latin
- Utilisation : mode batch ou interactif
- Principales commandes : `LOAD`, `STORE`, `DUMP`, `DESCRIBE`, `ILLUSTRATE`, `FILTER`, `DISTINCT`, `FOREACH...GENERATE`, `JOIN`, `GROUP`, `ORDER`, `SPLIT`
- Possibilité de créer des fonctions personnalisées en Java et de les utiliser via `REGISTER`

### Exemples de scripts
- Analyse de notes d’étudiants et calcul de statistiques par matière
- Transformation de noms en majuscules avec UDF
- Extraction des étudiants par mois de naissance

## MapReduce
- Deux fonctions principales : `map()` et `reduce()`
- Applications :
  - Comptage de mots, lettres ou initiales
  - Comptage par nom de famille
  - Calcul du TF-IDF en plusieurs étapes (MR1 à MR4)
  - Moteur de recherche simple avec top-10 fichiers pour un mot donné

## TF-IDF
1. `MR1` : Nombre d’occurrences par mot et fichier  
2. `MR2` : Nombre total de mots par fichier  
3. `MR3` : Nombre de fichiers par mot  
4. `MR4` : Calcul TF-IDF par mot et fichier

## Données utilisées
- Fichiers d’exemples : notes.txt, etudiants.txt  
- IMDB pour l’analyse des acteurs et films  
- Textes divers pour le comptage de mots et lettres

## Objectifs pédagogiques
- Comprendre l’exécution de scripts Pig sur Hadoop  
- Manipuler et transformer des données volumineuses  
- Développer des fonctions personnalisées pour Pig  
- Implémenter et enchaîner des jobs MapReduce complexes  
- Générer des indices et extraire des informations pertinentes avec TF-IDF
