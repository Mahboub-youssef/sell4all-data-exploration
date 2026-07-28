# Sell4All - Exploration de données

## Présentation du besoin

Sell4All est une entreprise de vente de vêtements d'occasion en ligne. 
Ce projet consiste à explorer et nettoyer les données clients (âge, pays, 
genre, dépenses) afin de préparer leur utilisation dans un futur projet 
de recommandation basé sur l'intelligence artificielle.

## Étapes suivies pendant la réalisation du projet

**Jour 1** : Installation de l'environnement (Miniconda, Jupyter Notebook, 
Pandas, Matplotlib), lecture du fichier CSV avec Pandas, exploration 
initiale des données avec `.head()` et `.info()`, rédaction de 
l'explication du résumé technique dans une cellule Markdown.

**Jour 2** : Calcul de la moyenne et de la médiane pour les colonnes Age 
et Customer spendings, calcul de la médiane d'âge par pays (bonus), 
création du graphique en barres des dépenses par pays, nettoyage des 
données (suppression des clients ayant dépensé moins de 10€, suppression 
des doublons), export du fichier CSV nettoyé, rédaction du README et 
publication sur GitHub.

Le projet a été réalisé en 2 jours sur les 3 jours prévus.

## Fonctionnalités développées

- Lecture du fichier CSV avec Pandas
- Affichage des 5 premières lignes (`head()`)
- Résumé technique du dataset (`info()`) avec explication
- Calcul de la moyenne et de la médiane (Age, Customer spendings)
- Calcul de la médiane d'âge par pays (bonus)
- Visualisation des dépenses par pays (graphique en barres)
- Nettoyage : suppression des clients ayant dépensé moins de 10€
- Nettoyage : suppression des doublons
- Export d'un fichier CSV nettoyé avec les colonnes Country, Age, 
  Gender, Customer spendings

## Difficultés rencontrées et solutions

- Erreur `CondaToSNonInteractiveError` lors de l'installation : résolue 
  en acceptant les conditions d'utilisation avec `conda tos accept`.
- Erreur `FileNotFoundError` lors de la lecture du CSV : le nom du 
  fichier n'était pas correct (manquait l'extension .csv).
- Erreur `NameError` : oubli des guillemets autour du nom de fichier 
  dans `read_csv()`.
- Le fichier CSV téléchargé se convertissait automatiquement en .xls 
  à cause d'Excel : résolu en renommant manuellement l'extension.

## Mode d'exécution du projet

**Prérequis** :
- Miniconda installé
- Bibliothèques : pandas, matplotlib

**Étapes** :
1. Cloner ce dépôt ou télécharger les fichiers
2. Ouvrir un terminal dans le dossier du projet
3. Lancer la commande : `jupyter notebook`
4. Ouvrir le fichier `exploration_sell4all.ipynb`
5. Exécuter les cellules dans l'ordre (Run All)
