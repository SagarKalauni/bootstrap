<div align="center">

# 🦁 Non-Parametric Bootstrapping — Statistical Resampling Masterclass
### **Lindenwood University — Interactive Data Science & Machine Learning Masterclass**

[![Live Interactive Lab](https://img.shields.io/badge/Launch_Interactive_Lab-Live_Demo-C5B358?style=for-the-badge&logo=googlechrome&logoColor=black)](https://sagarkalauni.github.io/bootstrap/)
[![Course](https://img.shields.io/badge/Course-MTH_34200-000000?style=for-the-badge&logo=academia&logoColor=C5B358)](#)
[![Author](https://img.shields.io/badge/Faculty-Sagar_Kalauni,_M.S.-1E293B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SagarKalauni)

</div>

---

## 📖 Overview

An interactive statistical laboratory demonstrating **Bradley Efron's Non-Parametric Bootstrap**. Students observe how resampling with replacement from a single observed sample approximates the sampling distribution, standard error, and confidence intervals of any estimator $\hat{\theta}$ without requiring parametric distributional assumptions.

> 🔗 **Launch the Live Interactive Application:** [**https://sagarkalauni.github.io/bootstrap/**](https://sagarkalauni.github.io/bootstrap/)

---

### 📐 Mathematical Formulation

Given an observed random sample $\mathbf{x} = (x_1, x_2, \dots, x_n)$ and a statistic of interest $\hat{\theta} = s(\mathbf{x})$, the non-parametric bootstrap generates $B$ independent resamples $\mathbf{x}^{*(b)} = (x_1^{*(b)}, \dots, x_n^{*(b)})$ drawn uniformly **with replacement** from $\mathbf{x}$.

- **Bootstrap Estimate of Standard Error:**
  $$\widehat{\text{SE}}_{\text{boot}}(\hat{\theta}) = \sqrt{\frac{1}{B - 1} \sum_{b=1}^{B} \left( \hat{\theta}^{*(b)} - \bar{\theta}^* \right)^2}, \quad \text{where } \bar{\theta}^* = \frac{1}{B}\sum_{b=1}^{B} \hat{\theta}^{*(b)}$$

- **$(1 - \alpha)$ Bootstrap Percentile Confidence Interval:**
  $$\text{CI}_{1-\alpha} = \left[ \hat{\theta}^*_{(\alpha/2)}, \; \hat{\theta}^*_{(1 - \alpha/2)} \right]$$

---

## ✨ Key Interactive Features

- **Animated Resampling with Replacement:** Watch individual observations get drawn (with duplicates and omissions) from the original sample.
- **Live Empirical Histogram Construction:** Build the bootstrap distribution across $B = 100, 1000, \dots$ Monte Carlo replicates.
- **Percentile & Normal-Theory Confidence Intervals:** Compare non-parametric bootstrap intervals against classical asymptotic intervals.
- **Flexible Estimators:** Test bootstrapping on the sample mean, median, variance, and trimmed statistics.

---

## 🎓 Pedagogical & Course Context

- **Institution:** Lindenwood University (*College of Science, Technology, and Health*)
- **Course Curriculum:** MTH 34200 — Probability & Mathematical Statistics II / DSCI 35600 — Machine Learning
- **Instructor & Author:** **Sagar Kalauni, M.S.** (*Full-Time Faculty in Data Science*)
- **Tech Stack:** HTML5, Tailwind CSS, **D3.js** (Dynamic Data Visualization), **MathJax** (LaTeX Mathematical Rendering), Vanilla ES6+ JavaScript (Zero-Dependency Client-Side Execution).

---

## 🚀 Running Locally

Because this visualizer is engineered as a self-contained, zero-build client-side application, you can run it immediately in any modern browser:

```bash
# Clone the repository
git clone https://github.com/SagarKalauni/bootstrap.git

# Navigate into the project directory
cd bootstrap

# Open index.html directly in your browser or serve locally:
python -m http.server 8000
```

---

## 🔗 Explore the Complete Interactive Masterclass Suite

| Module | Topic | Live Link |
| :--- | :--- | :---: |
| **Linear Regression** | Ordinary Least Squares & Residual Minimization | [Launch](https://sagarkalauni.github.io/linear-regression/) |
| **Logistic Regression** | Sigmoid Probabilities & Binary Cross-Entropy | [Launch](https://sagarkalauni.github.io/logistic-regression/) |
| **Regularization ($L_1 / L_2$)** | Lasso vs. Ridge Constraint Geometry | [Launch](https://sagarkalauni.github.io/Regularization/) |
| **K-Nearest Neighbors** | Instance-Based Learning & Distance Metrics | [Launch](https://sagarkalauni.github.io/knn/) |
| **Support Vector Machine** | Maximum-Margin Hyperplanes & Soft Margin $C$ | [Launch](https://sagarkalauni.github.io/support-vector-machine/) |
| **RBF Kernel SVM** | Non-Linear Kernel Trick & $(\gamma, C)$ Tuning | [Launch](https://sagarkalauni.github.io/rbf-kernel-svm/) |
| **Decision Tree (CART)** | Recursive Splitting, Gini & Entropy | [Launch](https://sagarkalauni.github.io/decision-tree/) |
| **Random Forest** | Bagging & Ensemble Variance Reduction | [Launch](https://sagarkalauni.github.io/random-forest/) |
| **Voting Classifier** | Hard Majority vs. Soft Probability Voting | [Launch](https://sagarkalauni.github.io/voting-classifier/) |
| **K-Means Clustering** | Lloyd's Algorithm, Voronoi & Elbow WCSS | [Launch](https://sagarkalauni.github.io/k-mean-clustering/) |
| **Confusion Matrix** | Precision, Recall, Specificity & $F_1$-Score | [Launch](https://sagarkalauni.github.io/confusion-matrix/) |
| **Confidence vs. Prediction Intervals** | Mean Response vs. Individual Uncertainty | [Launch](https://sagarkalauni.github.io/confidence-and-prediction-interval/) |
| **Bootstrapping** | Non-Parametric Resampling with Replacement | [Launch](https://sagarkalauni.github.io/bootstrap/) |
| **Q-Q Plot** | Gaussian Normality & Tail Diagnostics | [Launch](https://sagarkalauni.github.io/qq-plot/) |
| **Train-Test Split & CV** | Holdout Partitioning & $K$-Fold Cross-Validation | [Launch](https://sagarkalauni.github.io/split/) |
| **One-Hot Encoding** | Categorical Expansion & Dummy Variable Trap | [Launch](https://sagarkalauni.github.io/one-hot-encoding/) |

---

<div align="center">
  <sub>Developed with ❤️ for Data Science students by <a href="https://github.com/SagarKalauni">Sagar Kalauni</a> · <a href="https://sagarkalauni.github.io">Portfolio</a></sub>
</div>
