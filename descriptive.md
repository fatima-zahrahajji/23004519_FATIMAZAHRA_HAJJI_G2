# Description du jeu de données

## 1. Identification de la source

**Nom :** Données sur le PIB réel et le taux de chômage aux États-Unis.

**Organisme de diffusion :** FRED (Federal Reserve Economic Data), géré par la Federal Reserve Bank of St. Louis.

**Organismes d'origine :**
- Bureau of Economic Analysis (BEA) pour le PIB réel.
- Bureau of Labor Statistics (BLS) pour le taux de chômage.

**Liens des séries :**
- PIB réel : https://fred.stlouisfed.org/series/GDPC1
- Taux de chômage : https://fred.stlouisfed.org/series/UNRATE

**Date d'extraction :** 17/11/2026.

**Licence :** Les séries indiquent la mention « Public Domain: Citation Requested ». Les conditions d'utilisation de FRED et les éventuelles restrictions de redistribution doivent être vérifiées.

## 2. Caractéristiques des données

**Pays étudié :** États-Unis.

**Période étudiée :** 1990 T1 à 2026 T3 (période prévue, à vérifier selon les dernières observations disponibles).

**Fréquence initiale :**
- GDPC1 : trimestrielle.
- UNRATE : mensuelle.

**Unité d'observation :** Un trimestre.

**Taille du jeu de données :** À compléter après le chargement et le nettoyage des données dans Python.

## 3. Dictionnaire des variables

| Nom | Rôle | Type | Unité | Manquants |
|---|---|---|---|---|
| DATE | Identification | Date | Trimestre | À vérifier |
| GDPC1 | Variable initiale | Numérique | Milliards de dollars chaînés de 2017 | À vérifier |
| UNRATE | Variable initiale | Numérique | Pourcentage (%) | À vérifier |
| UNRATE_Q | Variable préparée | Numérique | Pourcentage (%) | À vérifier |
| GDP_Growth | Variable explicative (X) | Numérique | Pourcentage (%) | À vérifier |
| Delta_UNRATE | Variable cible (Y) | Numérique | Points de pourcentage | À vérifier |

## 4. Préparation prévue

Les données du taux de chômage étant mensuelles, elles seront transformées en données trimestrielles en calculant la moyenne des trois mois de chaque trimestre.

Ensuite, nous calculerons le taux de croissance trimestriel du PIB réel et la variation trimestrielle du taux de chômage.

Les valeurs manquantes et les éventuelles observations incomplètes seront également vérifiées avant l'application du modèle.
