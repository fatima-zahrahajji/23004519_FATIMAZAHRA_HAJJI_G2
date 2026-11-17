# 23004519_FATIMAZAHRA_HAJJI_G2
# F16 — Étude de la loi d'Okun

## 1. Présentation du projet

Ce projet porte sur l'étude de la relation entre la croissance économique et le chômage aux États-Unis, à travers la loi d'Okun.

L'objectif est de voir dans quelle mesure l'évolution du PIB réel peut expliquer la variation du taux de chômage.

## 2. Problématique

Dans quelle mesure la croissance du PIB réel permet-elle d'expliquer la variation du taux de chômage aux États-Unis ?

## 3. Données utilisées

Les données sont issues de FRED (Federal Reserve Economic Data).

Deux séries statistiques sont utilisées :

- GDPC1 : Produit intérieur brut réel des États-Unis.
- UNRATE : Taux de chômage des États-Unis.

## 4. Méthodologie

Il s'agit d'un problème d'apprentissage supervisé de type régression.

L'algorithme choisi est la régression linéaire simple (*Linear Regression*).

La variable explicative (X) est le taux de croissance trimestriel du PIB réel.

La variable cible (Y) est la variation trimestrielle du taux de chômage.

## 5. Organisation du projet

- `data/` : fichiers de données.
- `notebooks/` : notebook contenant le code et les explications.
- `figures/` : graphiques obtenus pendant l'analyse.
- `reports/` : rapport final du projet.
- `descriptive.md` : description du jeu de données.
- `requirements.txt` : bibliothèques Python utilisées.

## 6. Auteur

Projet individuel réalisé dans le cadre du cours de Machine Learning.
