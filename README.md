# Loan Pricing & Risk-Adjusted Return Analysis
### Credit Risk Analytics | Python | Scikit-learn | Basel III Aligned

---

## Project Overview

This project simulates a real-world credit risk workflow used by banks and NBFCs
to evaluate, grade, and price retail loans. Starting from raw loan application data,
the analysis builds a full pipeline from default prediction through to portfolio
profitability measurement using RAROC.

**Dataset:** [Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk)
| 307,511 loan applications | 8% default rate

---

## Business Objective

Most credit risk projects stop at building a model. This project goes further:

> *Can we use default predictions to price loans correctly — and prove the
> portfolio is profitable on a risk-adjusted basis?*

---

## Methodology

| Phase | Description |
|-------|-------------|
| 1 | Data loading & portfolio baseline assessment |
| 2 | Data cleaning & feature engineering (AGE, DTI, YEARS_EMPLOYED) |
| 3 | Exploratory Data Analysis — 3 targeted credit risk charts |
| 4 | PD Model — Logistic Regression with AUC 0.64 |
| 5 | Risk Grading — Percentile-based A to E grades |
| 6 | Loan Pricing — Rate = CoF + Expected Loss + OpEx + Margin |
| 7 | RAROC Analysis — Portfolio profitability vs hurdle rate |
| 8 | Business Recommendations |

---

## Key Findings

- **Age is the strongest default predictor** — borrowers aged 20–25 default
  at 12.5%, over 2.5x the rate of borrowers aged 60–70 (5%)
- **Mid-range loans (4–6L) carry peak default risk** — consistent with the
  middle market risk bulge phenomenon
- **Risk-based pricing generates consistent ₹12,000 net income per loan**
  across all risk grades when correctly calibrated
- **All grades exceed the 15% RAROC hurdle rate** — confirming even
  high-risk borrowers are profitably serviceable if priced correctly

---

## Concepts Applied

`Probability of Default (PD)` · `Loss Given Default (LGD)` · 
`Exposure at Default (EAD)` · `Expected Loss` · `RAROC` · 
`Economic Capital` · `Risk-Based Pricing` · `Basel III` · 
`Adverse Selection` · `Class Imbalance Handling`

---

## Tech Stack

- **Python** — Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Model** — Logistic Regression with manual class weighting
- **Preprocessing** — Sklearn Pipeline + ColumnTransformer

---

## How to Run

1. Download `application_train.csv` from
   [Kaggle](https://www.kaggle.com/competitions/home-credit-default-risk/data)
2. Place it in the same folder as the notebook
3. Run `Jupyter Notebook` → open `loan_pricing_raroc.ipynb`
4. Kernel → Restart & Run All

---

*Built by Vinit Singh | [LinkedIn](www.linkedin.com/in/vinit-singh-7b616a175)*
