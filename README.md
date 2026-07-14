# Waiter_Tips_Prediction
Ce projet a pour objectif d'analyser les facteurs qui influencent les pourboires laissés aux serveurs dans un restaurant, puis de développer un modèle de Machine Learning capable de prédire le montant du pourboire.

Le projet couvre l'ensemble des étapes d'un projet de Data Science :

- Analyse exploratoire des données (EDA)
- Visualisation des données
- Prétraitement des données
- Entraînement d'un modèle de Machine Learning
- Évaluation des performances du modèle


# Le problème
Le pourboire laissé à un serveur dépend de plusieurs facteurs : type de restaurant, nombre de convives, montant de l'addition, etc. Ce projet analyse un jeu de données réel de pourboires et entraîne un modèle de machine learning pour prédire le montant du pourboire.


# Le Dataset
Le dataset  contient le sinformations suivantes:
- Total Bill : montant total de la facture (en dollars)
- Tip : montant du pourboire (variable cible)
- Sex : sexe de la personne qui paie
- Smoker : fumeur ou non
- Day : jour de la semaine
- Time : déjeuner ou dîner
- Size : nombre de personnes à la table


#  Analyse exploratoire
Le notebook explore la relation entre le pourboire et :

- le montant de l'addition et la taille du groupe
- le sexe de la personne qui paie
- le fait de fumer ou non
- le moment du repas (déjeuner / dîner)
- le jour de la semaine


# Principaux constats

- Les pourboires les plus élevés sont observés le samedi.
- Ce sont globalement les hommes qui laissent le plus de pourboires.
- Les non-fumeurs laissent en moyenne plus de pourboires que les fumeurs.
- Les pourboires sont légèrement plus élevés au dîner qu'au déjeuner.

# Prétraitement des données
Avant l'entraînement du modèle, plusieurs étapes ont été réalisées :

- Encodage des variables catégorielles
- Séparation des données en ensembles d'entraînement et de test
- Sélection des variables explicatives

Variables utilisées :

Total Bill
Sex
Smoker
Day
Time
Size

Variable cible :

Tip


# Machine Learning
Un modèle de régression linéaire (scikit-learn) est entraîné pour prédire le pourboire à partir de : total_bill, sex, smoker, day, time, size.

# Technologies utilisées

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

# Resultats

Le modèle permet d'estimer le montant du pourboire à partir des caractéristiques de la commande et des clients. Les performances obtenues montrent qu'il est possible de modéliser la relation entre le montant de la facture, les caractéristiques des clients et le pourboire laissé au serveur.
