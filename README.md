# 💳 Prédiction du Défaut de Paiement des Cartes de Crédit  
# 💳 Credit Card Default Prediction

## 📌 Description

Ce projet a pour objectif de prédire si un client va faire défaut sur sa carte de crédit, en utilisant des techniques de machine learning.  
This project aims to predict whether a credit card client will default, using machine learning techniques.

---

## 📊 Données utilisées | Dataset

- **Source** : [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- **Fichier** : `default of credit card clients.xls`
- 30 000 clients avec informations démographiques, comportementales et financières.  
- 30,000 clients with demographic, behavioral, and financial information.

---

## 🧠 Étapes du projet | Project Steps

### 1️⃣ Chargement et exploration des données  
**Loading and exploring the data**
- `df.info()`, `df.describe()`, `value_counts()`
- Visualisations initiales (histogrammes, boxplots)

### 2️⃣ Nettoyage des données  
**Data Cleaning**
- Correction des valeurs incohérentes (`EDUCATION`, `MARRIAGE`)
- Suppression des doublons
- Vérification des valeurs manquantes

### 3️⃣ Visualisation  
**Data Visualization**
- Histogrammes d'âge et de sexe
- Boîtes à moustaches (`LIMIT_BAL`, `AGE`)
- Countplots et heatmaps

### 4️⃣ Préparation des données  
**Data Preparation**
- Séparation des variables (X, y)
- Normalisation avec `StandardScaler`
- Découpage en train/test (`train_test_split`)

### 5️⃣ Entraînement du modèle  
**Model Training**
- Modèle : `RandomForestClassifier`
- Apprentissage sur les données d'entraînement

### 6️⃣ Évaluation du modèle  
**Model Evaluation**
- `classification_report`, `confusion_matrix`
- Matrice de confusion avec Seaborn (heatmap)

### 7️⃣ Sauvegarde et rechargement  
**Saving and reloading**
- Sauvegarde du modèle avec `joblib.dump()`
- Chargement avec `joblib.load()`

---

## ⚙️ Librairies utilisées | Libraries

```python
pandas, numpy, matplotlib, seaborn, scikit-learn, joblib
