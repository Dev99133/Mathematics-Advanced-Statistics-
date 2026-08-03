# Spread Locator — A Statistical Distribution Analysis Model

**Duration:** 6 Hours &nbsp;|&nbsp; **Type:** Theory + Practical
**Domain:** E-commerce Transaction Analytics

## 🎯 Objective

To understand and apply the concepts of **probability distributions and spread analysis** on a real e-commerce transaction dataset — testing theoretical understanding and practical application of distribution types, Q-Q plots, statistical transformations, and probability functions.

## 📖 Project Scenario

Acting as a data analyst for an e-commerce platform, this project analyzes **daily transaction amounts** to determine whether customer transactions follow known statistical distributions, how to handle skewed data, and what probability insights can be derived for the business.

## 📂 Repository Contents

| File | Description |
|---|---|
| `Spread_Locator_Analysis.ipynb` | Fully executed Jupyter Notebook — Part B (all data analysis, model fitting, charts, and interpretations) |
| `Spread_Locator_Theory_PartA.pdf` | Part A — theoretical foundation, answering all 11 checklist questions with formulas and examples |
| `spread_locator_dataset.csv` | The transaction dataset used for analysis (220 records, Jan 2023) |
| `README.md` | This file |

## 🧩 Dataset Structure

| Field | Type | Description |
|---|---|---|
| `transaction_id` | UUID/String | Unique identifier for each transaction |
| `customer_id` | UUID/String | Unique identifier for each customer |
| `transaction_amount` | Float | Total amount of the transaction (₹) |
| `transaction_date` | Date | Date of the transaction |
| `transaction_count` | Int | Number of transactions made by a customer in a given week |
| `region` | String | Customer's geographic region (North, South, East, West) |
| `transaction_status` | String | Whether the transaction was successful or failed |

## 🔬 Analysis Performed (Part B)

1. **Bernoulli & Binomial fit** — `transaction_status` (success/fail) and weekly `transaction_count`
2. **Poisson fit** — number of transactions per day (and weekly count, for comparison)
3. **Log-Normal & Power-Law modelling** of `transaction_amount`
4. **Q-Q Plot** to test normality of raw vs. log-transformed amounts
5. **Box-Cox Transform** to stabilise variance and reduce skewness
6. **Z-scores** and probability of a transaction exceeding ₹5000
7. **PDF and CDF** plots for transaction amounts
8. **Conclusion**: identifying the best-fitting distribution for each variable and the resulting business insights

## 📊 Key Findings

- **`transaction_status`** → Bernoulli(p ≈ 0.445) — ~44.5% success rate.
- **Weekly `transaction_count`** → Best modeled as **Poisson(λ≈2.85)**, not Binomial (mean ≈ variance; χ² rejects Binomial at p≈0.00004, accepts Poisson at p≈0.71).
- **Daily transaction volume** → **Poisson(λ≈7.10)** (χ² test does not reject Poisson, p≈0.23).
- **`transaction_amount`** → **Log-Normal(μ≈8.00, σ≈0.47)** is an excellent fit (KS test p≈0.90); a plain Normal fit is strongly rejected (p≈0.0003).
- The tail of `transaction_amount` does **not** follow a strict Power-Law (curved log-log CCDF).
- Box-Cox optimal λ≈-0.18 (≈0), confirming log-scale is the natural transform for this data; skewness drops from 3.73 → ≈0 after transformation.
- **P(transaction > ₹5000):** Empirical ≈ 11.4%, Log-Normal model ≈ 13.8%, naive Normal model ≈ 20.5% (overestimates risk).

## 🛠️ How to Run

1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install numpy pandas scipy matplotlib seaborn
   ```
3. Open `Spread_Locator_Analysis.ipynb` in Jupyter Notebook / JupyterLab / VS Code and run all cells (the notebook already contains all outputs, so you can also just read it directly).
4. Refer to `Spread_Locator_Theory_PartA.pdf` for the theoretical explanations behind each technique used in the notebook.

## ✅ Submission Checklist

- [x] Practical implementation in Jupyter Notebook
- [x] All charts labeled with short interpretations under each result
- [x] GitHub repository with source code and documentation
- [x] PDF document explaining theory concepts with definitions
- [x] Descriptive README.md

---
*"Quality is our Motto." — Shaping "skills" for "scaling" higher...!!!*

