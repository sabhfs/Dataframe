# Bibliothèque d'Analyse de Données en C

Ce projet est une implémentation d'une structure de données de type **Dataframe** en langage C.
L'objectif est de reproduire les fonctionnalités basiques de bibliothèques haut niveau (comme Pandas en Python) mais en gérant manuellement la mémoire et les types pour une performance optimale.

## Fonctionnalités

* **Gestion de types dynamiques** : Supporte `INT`, `FLOAT`, `DOUBLE`, `STRING`, `CHAR`, etc. au sein d'une même structure grâce à des `unions`.
* **Insertion dynamique** : Allocation mémoire automatique lors de l'ajout de lignes ou colonnes.
* **Tri Avancé** : Implémentation de l'algorithme **QuickSort** pour trier les colonnes.
* **Recherche** : Recherche binaire optimisée sur les données.
* **Analyse** : Calculs statistiques de base et affichage formaté.

## Structure du Code

* `dataframe.c` : Gestion de la structure globale (tableau de colonnes).
* `column 2.0.c` : Cœur du projet. Définit l'union `Column_Type` et gère le stockage polymorphe.
* `sort.c` : Algorithmes de tri (Quicksort) et de recherche binaire.
* `main.c` : Fichier de test et démonstration des fonctionnalités.
