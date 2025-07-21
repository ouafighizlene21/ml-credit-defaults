# 💳 Prédiction du Défaut de Paiement des Cartes de Crédit / Credit Card Default Prediction

Ce projet utilise des techniques de Machine Learning pour prédire le défaut de paiement d’un client basé sur des données financières.  
The goal of this project is to predict credit card default using Machine Learning techniques on real-world data.

---

## 📊 Dataset

- **Source** : [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- **Nom du fichier** : `default of credit card clients.xls`
- Le jeu de données contient des informations démographiques et financières de 30 000 clients.
- The dataset includes demographic and financial features of 30,000 credit card clients.

---

## 🔍 Étapes du projet / Project Steps

### ✅ 1. Chargement et exploration des données  
*Loading and exploring data*
- Chargement depuis l'URL
- Exploration initiale : `info()`, `describe()`, `value_counts()`, histogrammes

### 🧹 2. Nettoyage des données  
*Data cleaning*
- Gestion des valeurs inconnues (EDUCATION, MARRIAGE)
- Suppression des doublons

### 📊 3. Visualisation  
*Data visualization*
- Histogrammes, boxplots, countplots
- Analyse de la distribution des variables

### 🤖 4. Préparation des données et Feature Scaling  
*Data preparation and scaling*
- Séparation X/y
- Normalisation avec `StandardScaler`
- Split en train/test

### 🌲 5. Entraînement du modèle  
*Model training*
- Utilisation de `RandomForestClassifier`
- Entraînement sur les données d’entraînement

### 📈 6. Évaluation du modèle  
*Model evaluation*
- Rapport de classification (`classification_report`)
- Matrice de confusion (`confusion_matrix`)
- Heatmap avec Seaborn

### 💾 7. Sauvegarde et chargement du modèle  
*Model saving and loading*
- Sauvegarde avec `joblib.dump()`
- Chargement avec `joblib.load()`

---

## 🛠️ Librairies utilisées / Libraries used

```python
pandas, numpy, matplotlib, seaborn, scikit-learn, imblearn, skorecard
