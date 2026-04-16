# 📊 R-Advanced-Consumer-Behavior-Analytics

[![Language: R](https://img.shields.io/badge/Language-R-blue.svg)](https://www.r-project.org/)
[![Tidyverse](https://img.shields.io/badge/Library-Tidyverse-red.svg)](https://www.tidyverse.org/)
[![Machine Learning](https://img.shields.io/badge/ML-K--Means%20%7C%20Random%20Forest-orange.svg)](https://cran.r-project.org/web/packages/randomForest/index.html)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

> **"Unlocking Consumer Insights through Statistical Modeling and Machine Learning in R."**
> 
> This project provides a deep dive into e-commerce consumer behavior, analyzing 3,900+ transactions to uncover the drivers of purchase amounts. Using a combination of **Exploratory Data Analysis (EDA)**, **Linear Regression**, **K-Means Clustering**, and **Random Forest**, this study delivers actionable strategic recommendations for retail optimization.

---

## 🚀 Project Highlights

- **Data-Driven Segmentation**: Identified 4 distinct customer clusters using K-Means to tailor marketing efforts.
- **Predictive Modeling**: Developed regression and Random Forest models to forecast purchase amounts with high accuracy.
- **Strategic Insights**: Discovered a "sweet spot" for pricing ($25-$35) and identified top-performing seasonal and regional trends.
- **Comprehensive Reporting**: Includes a detailed statistical report covering hypothesis testing (ANOVA, T-Tests) and model diagnostics.

---

## 🛠️ Tech Stack & Methodology

### 1. Data Preprocessing & EDA
- **Libraries**: `dplyr`, `ggplot2`, `tidyverse`, `corrplot`.
- **Techniques**: Missing value imputation, outlier treatment (95th percentile capping), and feature engineering (Loyalty Scoring, Discount Utilization).

### 2. Statistical Analysis
- **Hypothesis Testing**: Conducted T-Tests and ANOVA to validate regional and gender-based differences in spending.
- **Diagnostics**: Performed Breusch-Pagan tests for heteroscedasticity and Q-Q plots for normality.

### 3. Machine Learning Models
- **Linear Regression**: To identify key predictors of transaction value.
- **K-Means Clustering**: Segmenting the audience into High, Medium, and Low-value consumers.
- **Random Forest**: Evaluating feature importance to understand behavioral drivers.

---

## 📂 Repository Structure

- `marketing project R.R`: The complete R script containing data cleaning, visualization, and modeling.
- `rapport R fatma hammami (3).pdf`: The full analytical report with detailed findings and visualizations.
- `project_summary.md`: Executive summary of the strategic insights and methodology.
- `README.md`: This document.

---

## 📈 Key Findings

| Metric | Insight |
| :--- | :--- |
| **Price Sensitivity** | High concentration of purchases in the **$25 - $35** range. |
| **Top Region** | The **West** region leads in total purchase volume. |
| **Best Season** | **Fall** is the peak season for consumer engagement. |
| **Top Category** | **T-shirts** represent the most consistent high-performing item. |

---

## ✍️ Author
**Fatma Hammami**  
*Data Analyst & Business Strategist*

---

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
