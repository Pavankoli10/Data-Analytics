# Data Analytics & Inferential Statistics Portfolio

Welcome to my data analytics portfolio. This repository houses structural business analysis case studies, data processing steps, and practical implementations of inferential hypothesis testing.

---

## 📁 Repository Directory

### 🧠 [Inferential Statistics](./Inferential-Statistics/)
* Frameworks for statistical testing, calculation scripts for test statistics, boundary analysis, and probability distributions using `scipy` and `statsmodels`.

### 💼 [Projects](./Projects/)

#### 1. [Credit Card Spending Downturn Analysis](./Projects/Credit_Card_Spending_Analysis/) (Left-Tailed Z-Test)
* **Business Case:** Investigating if consumer economic shifts and pricing adjustments have significantly driven transaction counts below the historical baseline of **\$3,000**.
* **Methodology:** One-sample left-tailed Z-test (\(n=150\), \(\alpha=0.05\)).
* **Outcome:** **Rejected the Null Hypothesis (\(p = 0.0194\))**. Confirmed a statistically significant drop in baseline user spending.

#### 2. [Premium Spending Growth Validation](./Projects/Credit_Card_Spending_Growth_Analysis/) (Right-Tailed Z-Test)
* **Business Case:** Evaluating the performance of a newly launched credit card rewards program upgrade to prove if average transactions have expanded past a baseline of **₹2,500**.
* **Methodology:** One-sample right-tailed Z-test with Critical Value, P-Value, and Critical Sample Mean calculations (\(n=150\), \(\alpha=0.05\)).
* **Outcome:** **Failed to Reject the Null Hypothesis (\(p = 0.0692\))**. Observed transaction growth remains within the realm of normal variance; recommendations lean toward optimizing current program terms before scaling infrastructure limits.

---

## 🛠️ Global Tech Stack
* **Languages:** Python (Pandas, NumPy)
* **Statistical Computation:** Statsmodels (`weightstats.ztest`), SciPy (`stats.norm.cdf`, `stats.norm.ppf`)
* **Version Control:** Git, GitHub Desktop
