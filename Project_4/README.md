# Calculative Foundation

**Linear Algebra Analysis on a Student Performance Dataset**

Duration: 6 Hours &nbsp;|&nbsp; Type: Theory + Practical

## Objective

This project analyzes and transforms a student-performance dataset using **Linear
Algebra concepts** — vectors, matrices, decompositions, and dimensionality-reduction
techniques — to derive meaningful insights. It's a hands-on practice in mathematical
foundations widely applied in **Data Science, AI/ML, and Engineering**.

## Problem Statement

A research institute shared a dataset of **students' performance scores across
multiple subjects** (Math, Science, English, History, Computer). The task is to apply
Linear Algebra techniques to:

1. Represent and manipulate the data using vectors and matrices.
2. Perform advanced operations (dot products, cross products, vector projections, norms).
3. Interpret eigenvalues and eigenvectors to understand variance in the dataset.

## Repository Contents

| File | Description |
|---|---|
| `Calculative_Foundation.ipynb` | Full Jupyter Notebook implementation — all tasks below, executed with outputs, charts, and written interpretations. |
| `Calculative_Foundation_Theory.pdf` | Theory document defining every concept used (vectors, norms, dot/cross product, projection, matrix ops, determinant, inverse, line/plane/hyperplane, eigenvalues/eigenvectors, decompositions). |
| `student_performance.csv` | Dataset: 200 students &times; Math, Science, English, History, Computer scores, Average Score, and Category (Above/Below Average). |
| `README.md` | This file. |

## Tasks Covered

**Part A — Vector & Matrix Fundamentals**
- Represent each student's subject scores as a vector
- Norm-1 and Norm-2 of vectors
- Dot product and angle between two students' score vectors
- Cross product (3D subset of subjects)
- Projection of one vector onto another

**Part B — Matrix Operations**
- Form a students &times; subjects matrix
- Matrix addition and multiplication
- Transpose
- Determinant and Inverse

**Part C — Linear Transformations & Geometry**
- Line, Plane, and Hyperplane explained with respect to the dataset's dimensions
- Dimensionality increase: 2D &rarr; 3D &rarr; higher-dimensional hyperplane

**Part D — Eigenvalues & Decomposition**
- Eigenvalues and eigenvectors of the covariance matrix
- Eigen-decomposition verification (C = V&Lambda;V&#8315;&sup1;)

**Bonus — Additional Decompositions & Dimensionality Reduction**
- LU Decomposition
- Singular Value Decomposition (SVD)
- PCA (5 subjects &rarr; 2 dimensions)

## How to Run

```bash
git clone <this-repo-url>
cd calculative-foundation
pip install numpy pandas matplotlib scipy scikit-learn jupyter
jupyter notebook Calculative_Foundation.ipynb
```

Run all cells top to bottom — `student_performance.csv` must be in the same folder
as the notebook.

## Expected Outcome

By completing this project you will:
- Understand vector and matrix manipulation in real-world data.
- Apply norms, dot/cross products, and projections to performance data.
- Gain insights into eigenvalues/eigenvectors and their meaning.
- Build confidence using linear algebra foundations in applied statistics and
  machine learning.

## Video Link - [https://drive.google.com/file/d/1C2HpZy3zVmRUimxzzUTmTegKFZc2rdAs/view?usp=sharing]

## Author's Notes

- All charts are labeled with titles/axes, and every result is followed by a short
  written interpretation directly in the notebook.
- Theory concepts, formulas, and their meaning in this dataset's context are
  documented separately in `Calculative_Foundation_Theory.pdf`.

---
*"Quality is our Motto."*

