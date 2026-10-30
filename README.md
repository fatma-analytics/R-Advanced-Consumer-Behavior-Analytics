# Comportement d'achat des consommateurs — analyse statistique en R

**Question :** quels facteurs expliquent le montant d'achat des clients d'un site e-commerce, et quels segments de clients peut-on distinguer ?

Projet réalisé en R pendant mon Master : nettoyage des données, statistiques descriptives, tests statistiques, régressions et segmentation.

## Données

Jeu de données public **Customer Shopping Trends** (Kaggle) : 3 900 achats, 19 variables (âge, genre, région, catégorie, saison, montant, remise, code promo, abonnement, nombre d'achats précédents...).

Les données ne sont pas incluses dans le dépôt. Pour reproduire l'analyse, télécharger le fichier sur Kaggle et l'enregistrer sous `data/archive.csv`.

## Méthode

1. **Préparation** : suppression des valeurs manquantes, conversion des variables qualitatives, regroupement des États américains en 5 régions, création de variables binaires.
2. **Analyse descriptive** : distributions des montants, comparaisons par région, saison et catégorie (`ggplot2`, `corrplot`).
3. **Tests statistiques** :
   - test t (montant selon le genre, selon l'utilisation d'un code promo) ;
   - ANOVA et test de Tukey (montant selon la région) ;
   - test du khi-deux (région et abonnement) ;
   - test de Breusch-Pagan (hétéroscédasticité de la régression).
4. **Modélisation** : régression linéaire (avec interactions), régression logistique (utilisation d'un code promo), Random Forest (importance des variables).
5. **Segmentation** : K-Means, nombre de groupes choisi par la méthode du coude et l'indice de silhouette, ACP pour la visualisation.

## Principaux résultats

- Les achats se concentrent dans la tranche de **25 à 35 $**.
- La région **Ouest**, la saison d'**automne** et les **T-shirts** représentent les volumes d'achat les plus élevés.
- Les variables de comportement (achats précédents, mode de paiement) expliquent mieux le montant que les variables démographiques.

Le rapport complet, avec les sorties des tests et les graphiques, est dans `rapport R fatma hammami (3).pdf`. Une synthèse est disponible dans `project_summary.md`.

## Reproduire

```r
install.packages(c("tidyverse", "fastDummies", "corrplot", "randomForest",
                   "caret", "factoextra", "lmtest", "psych"))
source("marketing project R.R")
```

Le script s'exécute depuis la racine du dépôt (chemin relatif `data/archive.csv`) et fixe la graine aléatoire (`set.seed(123)`) pour que la segmentation soit reproductible.

## Fichiers

| Fichier | Contenu |
|---|---|
| `marketing project R.R` | Script complet : préparation, tests, modèles, segmentation |
| `rapport R fatma hammami (3).pdf` | Rapport d'analyse |
| `project_summary.md` | Synthèse des résultats |

**Auteure :** Fatma Hammami · Licence MIT
