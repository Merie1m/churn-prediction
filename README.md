\# 🎬 Churn Prediction — Streaming Platform



\## 📌 Objectif

Prédire les abonnés à risque de résiliation sur une plateforme de streaming

en utilisant des modèles de classification supervisée.



\## 📁 Structure du projet

churn-prediction/

├── data/

│   ├── raw/          # Dataset original

│   └── processed/    # Données nettoyées

├── notebooks/

│   ├── 01\_EDA.ipynb

│   ├── 02\_preprocessing.ipynb

│   └── 03\_modeling.ipynb

├── outputs/

│   ├── models/       # Modèles sauvegardés

│   └── predictions/  # CSV final des scores

├── dashboard/        # Fichiers Power BI

├── report/           # Rapport CRISP-DM

└── README.md



\## 🛠️ Technologies utilisées

\- Python 3.x, Jupyter Notebook

\- pandas, matplotlib, seaborn

\- scikit-learn, xgboost, imbalanced-learn

\- Power BI

\- Git / GitHub



\## 📊 Dataset

\- Source : \[Telco Customer Churn — IBM/Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

\- 7 043 clients, 21 variables



\## 🚀 Lancer le projet

```bash

pip install -r requirements.txt

jupyter notebook

```



\## 👥 Équipe

| Nom | Rôle |

|-----|------|

| ... | Data Scientist |

| ... | Data Analyst |

| ... | Project Manager |



\## 📈 Résultats

\- Meilleur modèle : \*\*XGBoost\*\*

\- AUC-ROC : \*\*> 0.80\*\*

