# Linear Algebra Coursework (UE24CS241A / UE24CS251B)

Comprehensive collection of applied computational linear algebra laboratory assignments, mathematical derivations, Jupyter/Colab notebooks, and datasets developed for the Linear Algebra course in the Computer Science & Engineering undergraduate curriculum at PES University.

---

## 🏛️ Curriculum & Architecture Structure

```
Linear Algebra Coursework
├── Unit 1: Linear Systems & Matched Filtering
│   ├── Vector Spaces, Subspaces & Linear Combinations
│   ├── Inner Products, Orthogonality & Signal Detection
│   └── Audio / Signal Matched Filtering (`Scores.mat`)
├── Unit 2: Matrix Decompositions & Recommender Systems
│   ├── Matrix Factorizations (LU, QR, SVD)
│   ├── Four Fundamental Subspaces (Row, Column, Null, Left-Null Space)
│   └── Collaborative Filtering Recommender Engine (`users_movies.mat`)
├── Unit 3: Orthogonal Projections & Least Squares Estimation
│   ├── Vector Projections & Normal Equations
│   ├── Best-Fit Hyperplane Fitting & Residual Minimization
│   └── Colab Numerical Simulations & Output Figures
└── Level 3: Jackfruit Project (Urban Traffic Flow Analysis)
    └── (Dedicated Repository: Traffic-Flow-Pattern-Detection-LA)
```

---

## 📂 Repository Contents

### 🔹 [Unit 1: Linear Systems & Matched Filtering](./Unit-1-Linear-Systems-and-Matched-Filtering/)
* **`Unit 1.ipynb`**: Interactive notebook exploring vector space foundations, linear combinations, matrix rank, linear independence, and matched filtering.
* **`Scores.mat`**: MATLAB matrix dataset representing score and signal vectors for empirical testing.
* **`Unit1Appendix.pdf`**: Theoretical derivations, problem sets, and mathematical foundations for Unit 1.

### 🔹 [Unit 2: Matrix Decompositions & Recommender Systems](./Unit-2-Matrix-Decompositions-and-Recommender-Systems/)
* **`Unit2.ipynb`**: Comprehensive computational notebook implementing:
  * **Four Fundamental Subspaces**: Computational verification of the Fundamental Theorem of Linear Algebra ($C(\mathbf{A})$, $N(\mathbf{A})$, $C(\mathbf{A}^T)$, $N(\mathbf{A}^T)$).
  * **Recommender Systems**: High-dimensional collaborative filtering analyzing user preference vectors and movie feature embeddings.
  * **Rank & Nullity**: Calculation of null space dimensions (nullity = 439) on sparse matrix data.
* **`users_movies.mat`**: High-dimensional user-item ratings matrix ($1.59\text{ MB}$) powering the movie recommender system.
* **`Unit_2_Linear_Algebra_Functions_updated.pdf`**: Mathematical definitions, function proofs, and algorithm specifications.

### 🔹 [Unit 3: Orthogonal Projections & Least Squares](./Unit-3-Projections-and-Least-Squares/)
* **`Unit_3_Appendix.pdf` & `Unit_3_Appendix.docx`**: Complete laboratory manual, problem sets, and derivation documentation covering projection matrices:
  
  $$\mathbf{P} = \mathbf{A}(\mathbf{A}^T \mathbf{A})^{-1}\mathbf{A}^T$$
  
  and least-squares approximation error analysis.
* **`colab-cell-outputs/`**: 5 high-resolution exported plot figures generated from Google Colab simulations demonstrating projection vectors, error residuals, and matrix transformations.

---

### 🍈 Level 3: Jackfruit Final Project (Urban Traffic Analysis)
* 🔗 **Dedicated Repository**: [**`Tanmayi-n14/Traffic-Flow-Pattern-Detection-LA`**](https://github.com/Tanmayi-n14/Traffic-Flow-Pattern-Detection-LA)
* Urban vehicular flow modeling using RREF, matrix rank reduction for sensor deployment optimization, and multivariate least squares traffic congestion prediction across arterial Bengaluru corridors.

---

## 🛠️ Software & Environment Setup

All notebooks can be executed using Google Colab or a local Jupyter environment:

```bash
pip install numpy scipy pandas sympy matplotlib jupyter
jupyter notebook
```

MATLAB `.mat` files are loaded natively in Python using `scipy.io`:
```python
import scipy.io as sio
data = sio.loadmat('users_movies.mat')
```

---

## 👤 Author
* **Tanmayi Nagabhairava** ([@Tanmayi-n14](https://github.com/Tanmayi-n14)) — `PES1UG24CS493`
* Department of Computer Science & Engineering, PES University
