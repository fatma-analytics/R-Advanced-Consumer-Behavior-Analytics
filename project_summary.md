# Analyse Avancée du Comportement des Consommateurs en E-Commerce (R)

## Objectif de l'Étude
Cette analyse porte sur un ensemble de données transactionnelles de 3900 lignes avec 19 variables. L'objectif est d'identifier les facteurs clés influençant le comportement d'achat des consommateurs pour optimiser les stratégies marketing et la gestion des stocks.

## Insights Majeurs
- **Sensibilité au Prix** : Les clients sont très sensibles aux prix situés dans la tranche de **25$ à 35$**.
- **Segments les plus Actifs** : La région **Ouest**, les **T-shirts** et la saison d'**Automne** présentent les volumes d'achat les plus élevés.
- **Facteurs Prédictifs** : Les comportements transactionnels (achats précédents, mode de paiement) sont de meilleurs prédicteurs du montant d'achat que les données démographiques pures.

## Méthodologie Statistique & Machine Learning
1.  **Nettoyage des Données** : Traitement des valeurs manquantes, gestion des valeurs aberrantes (capping au 95ème percentile) et ingénierie de variables (Indicateur de fidélité, Utilisation de remises).
2.  **Analyse Exploratoire (EDA)** : Visualisation des distributions de montants d'achat et des tendances saisonnières/régionales.
3.  **Modélisation de Régression** : Utilisation de la régression linéaire pour prédire le montant des achats et tests de diagnostic (Breusch-Pagan pour l'hétéroscédasticité).
4.  **Segmentation (Clustering)** : Application de l'algorithme **K-Means** pour segmenter les clients en 4 groupes distincts basés sur le montant d'achat, l'âge et l'historique.
5.  **Forêt Aléatoire (Random Forest)** : Évaluation de l'importance des variables pour la prédiction des comportements.

## Recommandations Stratégiques
- **Promotions Ciblées** : Focaliser les efforts sur les clients fidèles identifiés par le scoring.
- **Optimisation des Stocks** : Augmenter les stocks pour les segments populaires (T-shirts, Automne).
- **Marketing Saisonnier** : Intensifier les campagnes durant la période automnale.
