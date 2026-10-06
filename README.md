# credit_default_risk_analysis
# Credit Default Risk Analysis

##  Project Overview

Credit risk analysis is not only about identifying who may default, but also about understanding **what borrower characteristics are associated with higher or lower repayment risk**.

This project analyzes borrower and loan characteristics to answer a business-focused question:

> **How can we understand borrower risk patterns and identify meaningful risk segments?**

The objective is to move beyond analyzing individual variables and understand how financial burden, loan pricing, and employment stability interact to form different borrower risk profiles.

This project was developed as a **Data Analyst project**, with a focus on exploratory analysis, business interpretation, and risk segmentation rather than predictive machine learning.

---

##  Business Problem

A lending institution needs to understand its borrower portfolio and identify groups of borrowers that exhibit different levels of repayment risk.

The key questions addressed in this analysis are:

* What borrower and loan characteristics are associated with default?
* How does financial burden affect borrower risk?
* Does employment stability appear to differentiate borrower risk?
* How does interest rate relate to default patterns?
* Can multiple borrower characteristics be combined to create meaningful and interpretable risk segments?

### Business Objective

> **Understand borrower risk patterns and identify meaningful risk segments.**

---

##  Dataset

The dataset contains information about borrowers, their financial characteristics, loan characteristics, and whether the loan resulted in a default.

Key variables explored include:

* **Age**
* **Income**
* **Loan Amount**
* **Credit Score**
* **Months Employed**
* **Number of Credit Lines**
* **Interest Rate**
* **Loan Term**
* **DTI Ratio**
* **Employment Type**
* **Default**

The `Default` variable indicates whether the borrower defaulted on the loan.

---

##  Analytical Approach

The analysis follows a business-oriented exploratory workflow.

### 1. Data Understanding & Preparation

* Inspected the dataset structure and variables
* Checked data types and data quality
* Examined distributions of key numerical variables
* Reviewed categorical variables and borrower characteristics
* Prepared variables for meaningful comparison

### 2. Portfolio-Level Analysis

Established the overall default rate as a benchmark for understanding the portfolio.

> **Overall default rate: 11.61%**

This benchmark was then used to interpret differences between borrower groups.

### 3. Individual Risk Drivers

Analyzed how default patterns vary across important borrower and loan characteristics, including:

* DTI Ratio
* Interest Rate
* Employment Type
* Income
* Credit Score
* Loan characteristics

The analysis showed that individual variables provide useful signals, but **no single characteristic fully explains borrower risk**.

### 4. Risk Segmentation

The analysis was then extended from individual factors to combinations of borrower characteristics.

Three particularly interpretable dimensions were combined:

* **Interest Rate**
* **Employment Type**
* **DTI Ratio**

These combinations produced borrower profiles that could be compared using:

* Number of borrowers
* Number of defaults
* Default rate

This resulted in **64 borrower profiles**, allowing the analysis to move from isolated variable-level findings toward interpretable borrower segments.

---

##  Key Insight

The most important finding from the analysis is that borrower risk becomes more meaningful when **multiple characteristics are considered together**.

A broad pattern emerged across the borrower profiles:

### Relatively Lower-Risk Profile

**Low DTI + Low Interest Rate + Stable Employment**

This profile represents borrowers with comparatively lower financial burden, lower loan pricing, and more stable employment conditions.

### Relatively Higher-Risk Profile

**High DTI + Low Interest Rate + Unstable Employment**

This combination indicates greater financial pressure alongside weaker employment stability.

The analysis therefore suggests that:

> **Borrower risk is better understood through combinations of financial burden, loan pricing, and employment stability rather than through a single variable in isolation.**

---

##  Business Interpretation

These segments can help a lending organization understand its existing borrower portfolio more effectively.

For example:

### Lower-risk segments

Could represent borrowers with stronger financial stability and lower repayment pressure.

### Moderate-risk segments

May contain mixed characteristics where one favorable factor offsets another unfavorable factor.

### Higher-risk segments

Can highlight borrower groups where financial pressure and employment instability occur together.

The purpose of these segments is **not to automatically reject borrowers**, but to help the business understand where repayment risk is concentrated and where closer monitoring or further assessment may be appropriate.

---

## 📌 Important Limitation

This project is **descriptive and diagnostic**, not a predictive default model.

It does not attempt to predict the probability of default for a new borrower.

Instead, the analysis focuses on:

> **Understanding existing borrower risk patterns and creating interpretable risk segments from historical data.**

This distinction keeps the project aligned with a **Data Analyst / Business Analytics use case**.

---

##  Tools & Technologies

* **Python**
* **Pandas** — data manipulation and analysis
* **NumPy** — numerical operations
* **Matplotlib**
* **Seaborn** — data visualization
* **Jupyter Notebook**

---

##  Project Structure

```text
credit-default-risk/
│
├── data/
│   └── Loan_default.csv
│
├── notebooks/
│   └── credit_default_risk_analysis.ipynb
│
├── README.md
└── ...
```

---

##  Final Takeaway

The analysis demonstrates how a Data Analyst can move from raw lending data to a business-oriented understanding of credit risk:

**Borrower Data**
↓
**Exploratory Analysis**
↓
**Identify Risk Drivers**
↓
**Combine Relevant Characteristics**
↓
**Create Meaningful Risk Profiles**
↓
**Translate Patterns into Business Insights**

The final conclusion is that **risk is not adequately described by a single borrower characteristic**. Combining DTI, interest rate, and employment stability provides a more interpretable way to understand differences in borrower risk across the portfolio.

---

##  Project Focus

This project demonstrates practical skills in:

* Exploratory Data Analysis
* Business Problem Framing
* Risk Analysis
* Data Segmentation
* Data Visualization
* Pattern Identification
* Translating analytical findings into business insights

**Project Goal:**

> *Understand borrower risk patterns and identify meaningful risk segments.*

