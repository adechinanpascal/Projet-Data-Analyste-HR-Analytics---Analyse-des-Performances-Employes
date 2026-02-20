# 📊 HR Analytics — Analyse des Performances Employés

## 📝 Description

Ce projet réalise une analyse professionnelle des performances des employés à partir du dataset **HRDataset_v14** (311 employés, 36 variables). Il suit un workflow complet allant du nettoyage des données jusqu'aux insights business actionnables, en passant par des statistiques descriptives, des visualisations et une détection d'outliers.

---

## 🎯 Objectifs

- Identifier les **facteurs clés** liés à la performance des employés
- Détecter les **outliers** (top performers et sous-performers)
- Révéler les **disparités** entre départements et sources de recrutement
- Formuler des **recommandations business** concrètes et chiffrées

---

## 📁 Structure du projet
```
hr-analytics/
│
├── HR_Analytics_Performance.ipynb   # Notebook principal
├── HRDataset_v14.csv                # Dataset source
└── README.md                        # Documentation
```

---

## 🔍 Contenu du Notebook

| Section | Description |
|---|---|
| **1. Chargement & Nettoyage** | Import, conversion des dates, calcul de l'ancienneté, encodage du PerformanceScore |
| **2. Statistiques Descriptives** | Moyenne, médiane, IQR, skewness — globales et par département/position |
| **3. Visualisations** | Histogrammes, barres, pie chart, boxplots, scatter plots, heatmap |
| **4. Détection des Outliers** | Règle 1.5 × IQR sur PerformanceScore et Salary, analyse par sous-groupes |
| **5. Insights Business** | Performance par département, salary vs performance, ancienneté, recrutement |
| **6. Synthèse** | Tableau récapitulatif des insights avec actions prioritaires |
| **7. Avancé** | Dashboard interactif Plotly (optionnel) |

---

## 📊 Principaux Résultats

- **78,1%** des employés sont évalués *Fully Meets* → forte compression centrale des évaluations
- L'**engagement** est le facteur le plus lié à la performance (r = 0,58)
- Les **retards** sont le signal d'alarme le plus fort (r = −0,75 avec la performance)
- Les sous-performers affichent un taux de départ de **48%** vs 22% pour les top performers
- **Employee Referral** est la source de recrutement la plus performante (moyenne 3,10/4)
- **29 salaires outliers** (>$96 837) sans corrélation avec la performance

---

## 🛠️ Technologies utilisées

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-4C72B0)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-orange)
![SciPy](https://img.shields.io/badge/SciPy-1.11-8CAAE6?logo=scipy)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

---

## ⚙️ Installation
```bash
# Cloner le dépôt
git clone https://github.com/votre-username/hr-analytics.git
cd hr-analytics

# Installer les dépendances
pip install pandas numpy matplotlib seaborn scipy jupyter

# (Optionnel) Pour le dashboard interactif
pip install plotly

# Lancer le notebook
jupyter notebook HR_Analytics_Performance.ipynb
```

---

## 📂 Dataset

Le dataset utilisé est le **Human Resources Dataset** disponible sur Kaggle :  
🔗 [HRDataset_v14 — Kaggle](https://www.kaggle.com/datasets/rhuebner/human-resources-data-set)

**Variables clés :**
- `PerformanceScore` — Niveau de performance (PIP / Needs Improvement / Fully Meets / Exceeds)
- `Salary` — Salaire annuel en $
- `Department` — Département de l'employé
- `EngagementSurvey` — Score d'engagement (1–5)
- `DateofHire` — Date d'embauche (utilisée pour calculer l'ancienneté)
- `RecruitmentSource` — Source de recrutement

---

## 👤 Pascal Adechinan

Projet réalisé dans le cadre d'un cours de **Data Analysis avec Python**.
