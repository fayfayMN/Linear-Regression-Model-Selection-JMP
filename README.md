# 🏘️ Case Study: Analyzing Real Estate Appraisal Inconsistency
**STAT 311 | Data Analysis & Model Selection | Tampa, FL Market Study**

## 📌 Project Overview
[cite_start]This case study investigates a critical question in real estate equity: **Do property appraisers apply consistent valuation criteria across diverse neighborhoods?** Using a dataset of 1,264 residential transactions in Tampa, Florida, I built a series of hierarchical regression models to determine if location influences not just baseline prices, but the actual "valuation rate" of land and physical improvements[cite: 65, 82].

## 🧠 The "Gap" Analysis
The core objective was to identify if "blind spots" exist in standard appraisal methodologies. [cite_start]If the relationship between appraised values and sale prices differs significantly by neighborhood, it suggests inconsistent practices with profound implications for tax fairness and market efficiency[cite: 72].

## 🛠️ Technical Implementation
[cite_start]I utilized **JMP Statistical Software** to develop and compare five increasingly complex models[cite: 17, 30]:

* [cite_start]**Model 1:** Baseline first-order model (Land + Improvements)[cite: 31].
* [cite_start]**Model 2:** Main effects with neighborhood dummy variables[cite: 33].
* [cite_start]**Models 3-4:** Interaction models testing if Land or Improvement effects vary by location[cite: 35, 36].
* [cite_start]**Model 5 (Selected):** Full interaction model ($SALES \sim LAND + IMP + NBHD + LAND \times NBHD + IMP \times NBHD$)[cite: 37, 196].

### Model Comparison Metrics
To find the most parsimonious yet accurate model, I performed:
* [cite_start]**Global F-Tests** for overall significance[cite: 39].
* [cite_start]**Partial F-Tests** for nested model comparisons (Crucial for justifying complexity)[cite: 40, 150].
* [cite_start]**Adjusted $R^2$ and MSE Comparison** to evaluate goodness-of-fit[cite: 42, 160].

## 📈 Key Findings & Impact
* [cite_start]**Statistical Justification:** Model 5 achieved the highest Adjusted $R^2$ (0.9583) and lowest RMSE (81,403.59).
* [cite_start]**Proven Inconsistency:** Highly significant Partial F-tests ($p < 0.0001$) confirmed that both land and improvement valuation practices vary systematically across neighborhoods[cite: 199, 210].
* [cite_start]**Conclusion:** The analysis revealed that location affects both the level and the slope of property value, indicating neighborhood-specific factors that standard assessments may overlook[cite: 208].

## 🧰 Tech Stack
* [cite_start]**Analysis Tool:** JMP [cite: 17]
* [cite_start]**Methodology:** Hierarchical Regression, Interaction Modeling, Hypothesis Testing (F-tests, T-tests) [cite: 30, 105]
