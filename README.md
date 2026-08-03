# Mathematics for Data Science — Project Portfolio

A collection of applied **Probability & Statistics** and **Linear Algebra** projects,
each solving a real analytical problem end-to-end in a Jupyter Notebook: from raw
dataset to statistical/mathematical modelling, visualization, and written
interpretation of results.

## Repository Contents

| Notebook | Topic | Dataset |
|---|---|---|
| [`Expectation_Decider_Analysis_1.ipynb`](./Expectation_Decider_Analysis_1.ipynb) | Probability Theory | 200 Students Dataset |
| [`derivable_judgement_analysis.ipynb`](./derivable_judgement_analysis.ipynb) | Inferential Statistics & Hypothesis Testing | Public Health Dataset (1,000 records) |
| [`Spread_Locator_Analysis_Fixed.ipynb`](./Spread_Locator_Analysis_Fixed.ipynb) | Probability Distributions | E-commerce Transactions (220 records) |
| [`Calculative_Foundation.ipynb`](./Calculative_Foundation.ipynb) | Linear Algebra | Student Performance Dataset (200 records) |

---

## 1. Expectation Decider — Probability Analysis of Student Exam Performance

Predicts whether a student passes a competitive mathematics exam using probability
theory, based on study hours, attendance, group discussion participation, and
previous test scores.

**Covers:**
- Basics of probability, experiments, sample space, and events
- Empirical vs. theoretical probability
- Random variables & probability distributions
- Venn diagrams for compound events
- Contingency tables and joint/marginal/conditional probability
- Understanding relationships between variables
- Bayes' Theorem application
- Final summary of findings

## 2. Derivable Judgement — A Statistical Decision-Making Model

Uses inferential statistics on a public health dataset (age, weight, BMI, blood
pressure, smoking status, exercise frequency, diabetes, hypertension, cholesterol,
glucose) to judge which lifestyle/demographic factors are statistically associated
with health outcomes.

**Covers:**
- Confidence intervals for key numerical variables
- Hypothesis 1: Smoking status vs. Diabetes — Chi-square test of independence
- Hypothesis 2: BMI (diabetic vs. non-diabetic) — t-test
- Hypothesis 3: Age group vs. Blood pressure — ANOVA
- Covariance and correlation between Age and BMI
- Bonus: Exercise frequency vs. Hypertension — Chi-square test
- Summary of all hypothesis test results

## 3. Spread Locator — A Statistical Distribution Analysis Model

Analyzes e-commerce daily transaction data to identify which statistical
distributions best describe customer purchase behaviour, and derives
probability-based business insights.

**Covers:**
- Bernoulli distribution — transaction success/fail
- Binomial distribution — weekly transaction counts
- Poisson distribution — transactions per day
- Log-Normal & Power-Law modelling of transaction amounts
- Q-Q plots for testing normality
- Box-Cox transform for variance stabilisation
- Z-scores & probability of a transaction exceeding a set threshold
- PDF & CDF of transaction amounts
- Conclusion — best-fit distribution for the data

## 4. Calculative Foundation — Linear Algebra Analysis on Student Performance

Applies linear algebra to a student-performance dataset (Math, Science, English,
History, Computer scores) to represent, transform, and extract insight from the
data using vectors, matrices, and decompositions.

**Covers:**
- **Part A — Vector & Matrix Fundamentals:** representing scores as vectors,
  Norm-1/Norm-2, dot product & angle, cross product, vector projection
- **Part B — Matrix Operations:** forming a students × subjects matrix, addition &
  multiplication, transpose, determinant & inverse
- **Part C — Linear Transformations & Geometry:** line/plane/hyperplane, and how
  dimensionality increases from 2D → 3D → higher dimensions
- **Part D — Eigenvalues & Decomposition:** eigenvalues/eigenvectors of the
  covariance matrix, and verifying the eigen-decomposition
- **Bonus:** LU decomposition, Singular Value Decomposition (SVD), and PCA
  (reducing 5 subjects to 2 dimensions)

A companion theory document, `Calculative_Foundation_Theory.pdf`, defines every
concept and formula used in that notebook.

---

## Tech Stack

`Python` · `pandas` · `NumPy` · `SciPy` · `scikit-learn` · `Matplotlib` · `seaborn` ·
`matplotlib-venn` · `Jupyter Notebook`

## How to Run

```bash
git clone <this-repo-url>
cd <this-repo-folder>
pip install pandas numpy scipy scikit-learn matplotlib seaborn matplotlib-venn jupyter
jupyter notebook
```

> Each notebook expects its dataset CSV in the same folder — update the `pd.read_csv(...)`
> path near the top of a notebook if your file is located elsewhere.

## Structure & Approach

Every notebook in this repository follows the same format:
1. **Setup** — load libraries and the dataset
2. **Concept sections** — one per statistical/mathematical technique, each with a
   short theory note, the Python implementation, a labelled chart where relevant,
   and a written interpretation of the result
3. **Summary/Conclusion** — a consolidated takeaway from all analyses performed

---
*"Quality is our Motto."*
