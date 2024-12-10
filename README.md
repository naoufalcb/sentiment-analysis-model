# Analyse des Commentaires en Ligne et Classification Sentimentale

Ce projet vise à effectuer le scraping des commentaires d'articles en ligne, à analyser leur sentiment basé sur les votes, et à entraîner un modèle de machine learning pour prédire le sentiment de nouveaux commentaires. Voici les étapes principales de ce projet :

## 1. Collecte de Données
- Utilisation de `requests` et `BeautifulSoup` pour scraper les commentaires et les votes depuis une URL spécifique.
- Extraction des commentaires textuels et de leurs votes positifs.
- Stockage des données dans un DataFrame Pandas pour les étapes suivantes.

## 2. Prétraitement des Données
- Nettoyage des textes pour supprimer la ponctuation et les mots inutiles.
- Tokenisation et préparation des données textuelles avec des outils comme `NLTK`.
- Création d'une colonne pour stocker les textes prétraités.

## 3. Exploration des Données
- Analyse et visualisation des données pour identifier les tendances sentimentales basées sur les votes.
- Catégorisation des commentaires en trois sentiments : négatif, neutre, positif.
- Génération de graphiques pour visualiser la fréquence des sentiments et les mots les plus fréquents par sentiment.

## 4. Entraînement du Modèle
- Utilisation de `TfidfVectorizer` pour transformer les données textuelles en représentations vectorielles.
- Entraînement d'un modèle Naive Bayes pour la classification sentimentale.
- Création d'une méthode pour extraire les mots les plus fréquents selon les sentiments et filtrer les commentaires en conséquence.

## 5. Évaluation du Modèle
- Calcul de la précision et évaluation de la performance à l'aide de métriques telles que le rapport de classification.
- Validation sur l'ensemble de données initial pour mesurer l'efficacité du modèle.

## 6. Application du Modèle
- Prétraitement et vectorisation de nouveaux commentaires.
- Prédiction des sentiments pour ces commentaires à l'aide du modèle entraîné.
- Présentation des résultats sous forme lisible.

## Technologies Utilisées
- **Langages** : Python
- **Bibliothèques** :
  - Web scraping : `requests`, `BeautifulSoup`
  - Prétraitement : `NLTK`, `string`
  - Manipulation de données : `Pandas`
  - Visualisation : `Matplotlib`, `Seaborn`
  - Machine Learning : `Scikit-learn`

## Instructions
1. **Installation des dépendances** :
   - Installez les bibliothèques nécessaires en exécutant :
     ```bash
     pip install requests beautifulsoup4 nltk pandas matplotlib seaborn scikit-learn
     ```
2. **Exécution** :
   - Configurez l'URL de l'article dans le script.
   - Lancez le script pour effectuer le scraping, analyser les données, entraîner le modèle, et prédire les sentiments de nouveaux commentaires.
3. **Personnalisation** :
   - Remplacez l'URL cible pour analyser d'autres articles.
   - Ajustez les paramètres de prétraitement ou d'entraînement selon vos besoins.

## Résultats Attendues
- Rapport détaillé sur la répartition des sentiments et les mots-clés dominants.
- Modèle de classification capable de prédire le sentiment de nouveaux commentaires.
- Visualisations claires des tendances sentimentales dans les données collectées.

## Contact
Pour toute question ou suggestion, veuillez me contacter à [nchabaa3@gmail.com](mailto:nchabaa3@gmail.com).

---
**Note** : Ce projet est conçu pour une application en langue arabe, mais il peut être adapté pour d'autres langues avec des modifications mineures dans le prétraitement.
