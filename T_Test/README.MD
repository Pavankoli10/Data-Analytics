# Medical Insurance Cost Analysis: Two-Sample T-Test

This project performs a statistical analysis to determine if smoking status significantly impacts individual medical insurance charges. By utilizing a two-independent-sample t-test, the analysis evaluates whether the average insurance cost for smokers differs significantly from that of non-smokers.

---

## 📋 Problem Statement
Does smoking status significantly impact individual medical insurance costs? We use statistical hypothesis testing to determine if the average insurance charges for smokers are different from the average charges for non-smokers.

### Hypotheses
*   **Null Hypothesis (\(H_0\)):** \(\mu_1 = \mu_2\) 
    *   *There is no significant difference in the mean insurance charges between smokers and non-smokers.*
*   **Alternative Hypothesis (\(H_1\)):** \(\mu_1 \neq \mu_2\) 
    *   *There is a significant difference in the mean insurance charges between smokers and non-smokers.*

---

## 📊 Dataset Overview
The dataset (`insurance.csv`) consists of **1,338 rows** and **7 columns**:

*   `age`: Age of the primary beneficiary.
*   `sex`: Insurance contractor gender (female, male).
*   `bmi`: Body mass index (\(kg / m^2\)).
*   `children`: Number of dependents covered by health insurance.
*   `smoker`: Smoking status (yes, no).
*   `region`: The beneficiary's residential area in the US.
*   `charges`: Individual medical costs billed by health insurance (Target Variable).

---

## 🛠️ Implementation & Libraries
The analysis is implemented in Python using two major statistical libraries to validate the consistency of the results:
1.  **SciPy (`scipy.stats`)**: Used to perform Welch's T-test (unequal variances assumed).
2.  **Statsmodels (`statsmodels.stats.api`)**: Used to perform a standard independent t-test.

### Key Outputs

| Library | T-Statistic | P-Value | Decision (\(\alpha = 0.05\)) |
| :--- | :--- | :--- | :--- |
| **SciPy** (Welch's) | `32.7519` | `5.8894e-103` | **Reject \(H_0\)** |
| **Statsmodels** | `46.6649` | `8.2714e-283` | **Reject \(H_0\)** |

---

## 💡 Conclusion
Because the p-value in both tests is well below the significance level (\(\alpha = 0.05\)), **we reject the Null Hypothesis**. 

There is overwhelmingly strong statistical evidence that the true mean medical insurance charges for smokers are significantly different from the true mean charges for non-smokers.

---



