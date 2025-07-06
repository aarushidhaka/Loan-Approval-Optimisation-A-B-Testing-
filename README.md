# A/B Testing for AI-Powered Loan Approval System Optimisation

This project evaluates an AI-powered loan approval model using **A/B testing** to assess its impact on financial risk management. The analysis focuses on reducing **Type II errors** (approving bad loans) and improving overall decision accuracy for a consumer lending company.  

The project was part of the *Advanced Data Analysis* module at Warwick Business School.

---

## 📂 Repository Contents

| File                         | Description                                                                                      |
|-------------------------------|--------------------------------------------------------------------------------------------------|
| `final_version.Rmd`          | RMarkdown file containing data cleaning, hypothesis testing, and visualization code.            |
| `Group17 (1).pdf`            | Final report outlining methodology, business impact, and recommendations.                       |
| `ADAproject_2025_data.csv`   | Dataset containing experimental loan review results (control vs. treatment groups).             |

---

## 📝 Project Overview

- **Objective**: Assess whether an AI model can reduce financial losses from bad loans by minimizing false negatives (Type II errors) and improving loan officer confidence.  
- **Key Features**:
  - Hypothesis testing to compare control and treatment groups.  
  - Metrics: Type I & Type II error improvements, agreement rate, revision rate, confidence scores.  
  - Visualizations: Histograms, density plots, and trend analyses for performance metrics.  

---

## 📊 Results & Insights

| Metric                   | Improvement (Treatment vs Control) | Significance (p-value) |
|---------------------------|-------------------------------------|-------------------------|
| **Type II Errors**        | -0.21                              | ✅ Significant (p=0.0026)|
| **Type I Errors**         | -0.56                              | ✅ Significant (p<0.0001)|
| **Agreement Rate**        | +0.14                              | ✅ Significant          |
| **Revision Rate**         | +0.20                              | ✅ Significant          |
| **Confidence (Final)**    | +15.3                              | ✅ Significant          |
| **F1 Score**              | +0.06                              | ✅ Significant          |

- The AI model significantly reduced risky loan approvals and boosted officer confidence.  
- Recommended phased deployment for larger sample validation.  

---

## 🛠️ Tools & Techniques
- **Languages**: R  
- **Libraries**: ggplot2, dplyr, tidyr, caret  
- **Techniques**: A/B Testing, T-tests, Cohen’s d for effect size, Power Analysis  
- **Visualization**: Histograms, Density Plots, Trend Analysis  

---

## 📁 File Descriptions

### `final_version.Rmd`
- Contains:
  - Data preprocessing and filtering.  
  - Hypothesis testing (T-tests) for primary and secondary metrics.  
  - Effect size calculation and sample size estimation.  
  - Visualizations to compare Control vs. Treatment groups.  

---

### `Group17 (1).pdf`
- Report detailing:
  - Experimental setup and key objectives.  
  - Business impact analysis for financial decision-making.  
  - Recommendations for AI model deployment and improvement.  

---

### `ADAproject_2025_data.csv`
- Dataset:
  - **Rows**: 470 loan officer decisions  
  - **Columns**:  
    - `Variant` (Control/Treatment group),  
    - `typeI_init`, `typeII_init` (Initial Errors),  
    - `typeI_fin`, `typeII_fin` (Final Errors),  
    - Agreement and confidence metrics.  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/aarushidhaka/Loan-Approval-Optimisation-A-B-Testing-.git
   cd AI-Loan-Approval-A-B-Testing
2. Open final_version.Rmd in RStudio.
3. Knit the file to HTML or PDF to view the report.
