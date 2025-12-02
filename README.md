
**Projet d'analyse de données RH**  
**Imen Abdelkader** – 2024  

Analyse approfondie d’un jeu de données RH contenant plus de **15 000 employés** afin d’identifier les facteurs clés du turnover et proposer des **recommandations actionnables** pour améliorer la rétention.

![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776ab?style=flat&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=flat&logo=matplotlib&logoColor=black)

## Objectif du projet

Comprendre **pourquoi les employés quittent l’entreprise** et fournir aux RH des leviers concrets pour **réduire le turnover**.

## Principales questions traitées

- Quels sont les profils types des employés qui partent ?
- Quel impact de la satisfaction, de la charge de travail, des promotions, du salaire et de l’ancienneté ?
- Existe-t-il des départements plus touchés ?
- Quelles actions prioritaires pour améliorer la rétention ?

## Dataset (HR_SBA_Software.csv)

| Variable                | Description                                    | Type          |
|-------------------------|------------------------------------------------|---------------|
| satisfaction_level      | Niveau de satisfaction (0-1)                   | Float         |
| last_evaluation         | Dernière évaluation de performance (0-1)       | Float         |
| number_project          | Nombre de projets                              | Int           |
| average_montly_hours    | Heures mensuelles moyennes                     | Int           |
| time_spend_company      | Ancienneté (années)                            | Int           |
| Work_accident           | Accident du travail (0/1)                      | Binary        |
| left                    | A quitté l’entreprise (0/1) – **cible**        | Binary        |
| promotion_last_5years   | Promotion dans les 5 dernières années (0/1)    | Binary        |
| sales / department      | Département                                    | Catégorique   |
| salary                  | Niveau de salaire (low/medium/high)            | Catégorique   |

## Principaux résultats

- **Turnover global : 23,8 %**
- Les employés partent principalement pour **deux raisons extrêmes** :
  - Charge de travail très élevée (> 240 h/mois) ou très faible (< 150 h/mois)
  - Ancienneté de 3 à 5 ans (pic à 4 ans)
- Départements les plus touchés : **sales (27,6 % des départs)**, **technical**, **support**
- **Management** et **RandD** ont les meilleurs taux de rétention grâce à des salaires plus élevés et plus de promotions
- Les promotions sont très rares (seulement **2 %** des employés promus en 5 ans)

## Recommandations concrètes (prêtes à présenter aux RH)

1. **Équilibrer la charge de travail** → viser 166-215 heures/mois
2. **Augmenter fortement les promotions** (objectif 5-8 % par an) dans les départements sales, technical, hr, accounting
3. **Revaloriser les salaires** des postes techniques et support (trop de "low salary")
4. **Programme de fidélisation ciblé** pour les employés à 3-5 ans d’ancienneté (primes, évolution de poste)
5. **Actions spécifiques par département** (sales et technical en priorité)

## Contenu du repository
.
├── HR_SBA_Software.csv                  # Jeu de données complet
├── Projet Analyse des données.ipynb     # Notebook Jupyter (analyses + visualisations)
└── README.md                            # Ce fichier
text## Visualisations clés (exemples dans le notebook)

- Distribution du turnover par département/salaire
- Courbe du turnover selon les heures mensuelles (forme en U très nette)
- Analyse en composantes principales (PCA) expliquant les deux clusters de départs
- Heatmaps, boxplots, violin plots, etc.

## Comment exécuter le projet


# 1. Cloner le repo
git clone https://github.com/ton-pseudo/HR-Turnover-Analysis.git
cd HR-Turnover-Analysis

# 2. Créer un environnement (optionnel mais recommandé)
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate

# 3. Installer les dépendances
pip install pandas seaborn matplotlib scikit-learn

# 4. Ouvrir le notebook
jupyter notebook "Projet Analyse des données.ipynb"
N’hésite pas à star le repo si le sujet People Analytics / RH data-driven t’intéresse !
textCopie-colle tout ça → ton repo sera immédiatement propre, professionnel et très bien valorisé sur ton CV ou ton portfolio.
Tu veux que je te génère aussi une belle image de couverture (banner) pour le repo ? 😊7.5sin eenglish and max 350 car pour descriptionGitHub Repository Name
HR-Turnover-Analysis
GitHub Description (copy-paste, 248 characters)
textComprehensive HR analytics project to reduce employee turnover using a 15,000+ record dataset. Includes EDA, visualizations, PCA, and actionable insights on satisfaction, workload, promotions, and salary. Recommendations to improve retention. By Imen Abdelkader & Mohamed Amine Dammak (Dec 2025)
Full English README.md (copy-paste ready)
Markdown# HR Turnover Analysis – Data-Driven Retention Insights

**HR Analytics Project**  
**Imen Abdelkader & Mohamed Amine Dammak** – December 2025  

In-depth analysis of a 15,000+ employee HR dataset to understand why people leave and how to improve retention.

![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776ab?style=flat&logo=python&logoColor=white)

## Project Goal
Identify key factors driving employee turnover and provide clear, actionable recommendations for HR to boost retention.

## Key Questions Answered
- Who leaves and why? (satisfaction, workload, promotions, salary, tenure)
- Which departments have the highest turnover?
- How do promotions and accidents affect retention?
- What is the ideal workload to minimize departures?

## Dataset (HR_SBA_Software.csv)
- 10 features: satisfaction, evaluation, projects, monthly hours, tenure, accidents, turnover (target), promotions, department, salary
- Turnover rate: 23.8%

## Main Findings
- Two main departure profiles: overworked (>240h/month) or under-challenged (<150h/month)
- Peak turnover at 3-5 years of tenure
- Highest turnover in Sales, Technical, and Support
- Management and R&D retain best (higher salaries & promotions)
- Only 2% of employees promoted in 5 years

## Recommendations
1. Balance workload (target 166-215 hours/month)
2. Increase promotions (aim for 5-8% annually) in high-risk departments
3. Raise salaries in Technical and Support roles
4. Launch retention programs for employees with 3-5 years tenure

## Repository Contents
.
├── HR_SBA_Software.csv              # Full dataset
├── Projet Analyse des données.ipynb # Jupyter notebook (EDA + visuals)
└── README.md                        # This file
text## How to Run

git clone https://github.com/your-username/HR-Turnover-Analysis.git
cd HR-Turnover-Analysis
pip install pandas seaborn matplotlib scikit-learn
jupyter notebook "Projet Analyse des données.ipynb"
Star the repo if you like HR analytics! Perfect for data analyst or people analytics portfolios.
