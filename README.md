# 💼 BCG X Data Science Job Simulation — Forage

My completed work from the **BCG X Data Science Job Simulation** hosted on [Forage](https://www.theforage.com/simulations/bcg/data-science-ccdz). This simulation replicates a real-world consulting project at BCG X, working through the full data science lifecycle — from business problem framing to a production-ready predictive model — for a fictional energy utility company called **PowerCo**.

---

## 🏢 Business Context

**Client:** PowerCo — a major gas and electricity utility company serving corporate, SME, and residential customers across Europe.

**Problem:** Market liberalization has caused significant customer churn, especially in the SME segment. PowerCo partnered with BCG X to diagnose why customers are leaving and predict which ones are at risk.

**Hypothesis:** Churn is primarily driven by **price sensitivity**. The head of the SME division is considering offering a **20% discount** to at-risk customers to prevent them from churning.

**Goal:** Build a predictive model to identify customers likely to churn and provide data-driven recommendations on whether the discounting strategy makes business sense.

---

## 📁 Repository Structure

```
BCG-X-data-science-job-simulation/
│
├── Task 2 - eda_starter.ipynb                        # My EDA work (starter notebook)
├── Task 2 - Model Answer - EDA (2).ipynb             # BCG model answer for EDA
│
├── Task 3 - feature_engineering.ipynb                # My feature engineering work
├── Task 3 - Model Answer - Feature Engineering.ipynb # BCG model answer for feature engineering
├── Task_3_feature_engineering_complete.ipynb         # Completed feature engineering notebook
│
├── Task 4 - modeling_starter.ipynb                   # My modeling work (starter notebook)
├── Task 4 - Model Answer - Modeling.ipynb            # BCG model answer for modeling
|   
|   Task 5 - ppt for explain the full work overview
│
└── README.md
```

> All work is in Jupyter Notebooks (100% Python). Each task has both my working notebook and the official BCG model answer for comparison.

---

## 🗺️ Simulation Tasks

### Task 1 — Business Understanding & Hypothesis Framing *(no notebook)*
Understood the client's situation and formulated the data science hypothesis. Key output: a structured email to the Associate Director outlining:
- How to test the price sensitivity hypothesis
- What data is needed from the client
- Which analytical models to apply

---

### Task 2 — Exploratory Data Analysis (EDA)
**Notebook:** `Task 2 - eda_starter.ipynb`

Deep dive into PowerCo's customer and pricing datasets to understand behaviour patterns and churn drivers.

Key activities:
- Loaded and profiled customer data — data types, missing values, descriptive statistics
- Visualised distributions of key features (usage, pricing, contract tenure)
- Investigated the correlation between **price changes** and **churn rates**
- Identified potential churn indicators through visual analysis
- Summarised key findings and suggested additional data sources to enrich the analysis

**Libraries used:** `pandas`, `numpy`, `matplotlib`, `seaborn`

---

### Task 3 — Feature Engineering
**Notebooks:** `Task 3 - feature_engineering.ipynb` / `Task_3_feature_engineering_complete.ipynb`

Transformed the raw, cleaned dataset into a set of powerful features for the ML model.

Key activities:
- Engineered a key predictive feature: **difference between off-peak prices in December and January** of the preceding year (a proxy for price sensitivity)
- Extracted date-based features: activation year, renewal month, contract length in days
- Removed irrelevant columns (unique identifiers, redundant date fields)
- Merged customer and pricing datasets into a single modelling-ready DataFrame
- Evaluated feature importance and justified engineering decisions

**Libraries used:** `pandas`, `numpy`, `scikit-learn`

---

### Task 4 — Predictive Modelling & Evaluation
**Notebook:** `Task 4 - modeling_starter.ipynb`

Built and evaluated a machine learning model to predict customer churn.

Key activities:
- Trained a **Random Forest Classifier** on the engineered feature set
- Evaluated model performance using accuracy, precision, recall, and F1-score
- Analysed feature importances to understand the strongest churn signals
- Assessed whether offering a 20% discount to predicted churners is financially viable
- Prepared an **executive summary / abstract slide** with findings and business recommendations

**Libraries used:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Jupyter Notebook | Interactive development |
| pandas / numpy | Data manipulation |
| matplotlib / seaborn | Data visualisation |
| scikit-learn | Machine learning (Random Forest, metrics) |

---

## 📊 Key Outcomes

- Identified **price sensitivity** as a significant driver of SME customer churn
- Engineered features that meaningfully improved model predictive power
- Built a Random Forest model with strong churn prediction performance
- Produced actionable business recommendations: targeting high-risk customers with a 20% discount as a cost-effective retention strategy

---

## 🎓 About the Simulation

The **BCG X Data Science Job Simulation** on Forage is an 8–9 hour self-paced program that mirrors real work at BCG X — the tech-focused unit of Boston Consulting Group. Completing it demonstrates:

- Ability to frame business problems as data science hypotheses
- Proficiency in EDA, feature engineering, and ML modelling
- Skill in communicating technical findings to business stakeholders

Upon completion, participants receive a **certificate** verifiable by BCG recruiters.

---

## 🧑‍💻 Author

**Harshvardhan**
- GitHub: [@harshvardhan7709](https://github.com/harshvardhan7709)

---

## 📄 License

This repository contains personal simulation work for educational and portfolio purposes. All dataset rights belong to BCG / Forage.
