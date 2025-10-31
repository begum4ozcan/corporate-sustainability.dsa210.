# 🌍 Corporate Environmental Impact Analysis
**Course:** DSA 210 Introduction to Data Science  
**Term:** Fall 2025–2026  
**Student:** Begüm Özcan  

---

## 🧭 1. Project Proposal & Motivation
In recent years, corporate environmental responsibility has emerged as a critical dimension of business strategy, regulatory policy, and investor scrutiny. Firms are increasingly expected not only to generate financial value but also to minimize their environmental footprint — measured through greenhouse-gas emissions, energy and water usage, waste production, and resource intensity.

This project aims to analyze how **company features** — such as size, industry, and country development level — influence **corporate environmental impact**, focusing especially on **Turkish firms** compared to global peers. The core research question is:

**How do firm size, industry sector, and national development indicators (such as GDP per capita) influence a firm’s environmental impact score, and how do Turkish firms compare with global peers?**

**Motivation & Importance:**  
- **Relevance:** Understanding drivers of corporate environmental performance is valuable for business strategy, policy, and sustainable investment.  
- **Originality:** While much research focuses on global trends, few studies examine Turkish companies specifically. This provides a unique perspective and opportunity for comparative analysis.  
- **Data Science Practice:** The project provides a complete data science workflow experience — from data collection and cleaning, to exploratory analysis, hypothesis testing, and machine learning modeling.  
- **Insights & Applications:** Results may guide firms, investors, and policymakers in understanding patterns and predictors of environmental impact.

**Goals:**  
- Explore key relationships between firm characteristics and environmental impact.  
- Visualize patterns across industries, countries, and time.  
- Build predictive machine learning models for environmental impact scores.  
- Highlight Turkey-specific trends in comparison to global data.

---

## 📊 2. Data to Be Used

### Primary Dataset
- **Title:** Open Access Dataset of Corporate Environmental Impacts (2010–2018)  
- **Source:** [Corporate Sustainability Initiative / Harvard Impact‑Weighted Accounts Project] (link to dataset)  
- **Description:** Approximately 13,000 firm-year observations across multiple countries and industries. Includes metrics such as greenhouse gas emissions, water and energy consumption, and environmental intensity ratios.  
- **Key Features:** Firm identifier, year, country, industry sector, environmental metrics. Time span: 2010–2018.

### Enrichment Datasets
- **Country-level indicators:** GDP per capita, population, renewable energy share (World Bank).  
- **Human development metrics:** HDI (UN Data / Human Development Reports).  
- **Optional firm financials:** Revenue, total assets, and market capitalization from public sources.  
- **Policy or regional indicators:** Environmental regulation strength or climate risk indices if available.

**Purpose of Enrichment:**  
Merging firm-level data with country-level and financial context allows for deeper analysis of *why* firms perform better or worse environmentally, including Turkey-specific patterns. Subsets of Turkish firms will be analyzed for detailed comparison.

---

## ⚙️ 3. Data Collection & Preparation Plan

**Step 1 — Download Datasets:**  
- Primary corporate environmental impact dataset (`data/raw/`).  
- Country-level GDP, population, and HDI data (`data/raw/`).  
- Optional firm financial data (`data/raw/firm_financials/`).  

**Step 2 — Data Integration:**  
- Match company data with country indicators using the `country` field.  
- Add derived features (e.g., GDP group classification: high, middle, low income).  

**Step 3 — Data Cleaning:**  
- Handle missing values via imputation or row removal.  
- Convert text fields into categorical or numeric variables.  
- Standardize company-level metrics for consistent comparison.  

**Step 4 — Exploratory Data Analysis (EDA):**  
- Generate summary statistics and correlations.  
- Visual comparisons: Turkey vs global peers; industry comparisons.  
- Formulate initial hypotheses regarding industry and regional effects.  

**Step 5 — Hypothesis Testing:**  
- Test if higher GDP per capita countries have lower environmental impact scores.  
- Compare Turkish firms to the global average.  
- Compare industries (manufacturing/energy vs technology/services).  

**Step 6 — Machine Learning Modelling:**  
- Prediction target: environmental impact score (continuous) or categories (low/medium/high).  
- Baseline and advanced models: Linear Regression, Random Forest, Gradient Boosting.  
- Evaluate models and interpret feature importance (SHAP values if possible).  

**Step 7 — Reporting & Visualization:**  
- Save figures in `figures/` with captions and descriptions.  
- Prepare final report summarizing motivation, methods, findings, limitations, and future work.  
- Optional: create an interactive dashboard for exploration.  

**Step 8 — Version Control & Tools:**  
- Use GitHub for all code and commits (weekly recommended).  
- Python as primary language; include `requirements.txt` for dependencies.  
- Document AI assistance in `AI_usage.md` if any.

---

## 🗓️ Timeline & Milestones

| Date | Milestone |  
|------|-----------|  
| 31 Oct 2025 | Submit project proposal (this README) |  
| 28 Nov 2025 | Complete data collection, cleaning & EDA |  
| 02 Jan 2026 | Apply machine learning models and evaluate results |  
| 09 Jan 2026 | Submit final repository (code + report + visuals) |  
