# Decision Intelligence: Classification Models Across Banking, E-Commerce & Industrial Systems

> Built and compared classification models across banking, e-commerce, and industrial systems to optimize risk prediction, competitiveness forecasting, and alarm intelligence.

**Author:** Amisha Farhana Shaik  
**Project Type:** Classification Modeling | Decision Trees | kNN | Predictive Analytics  

---

## Business Context

Organizations across industries rely on predictive classification models to improve decision-making.

This project applies machine learning models to three real-world scenarios:

1. Predicting personal loan adoption (Banking)
2. Forecasting auction competitiveness (E-commerce)
3. Detecting alarm chattering in industrial systems (Energy / Manufacturing)

The goal across all cases was to improve predictive accuracy while aligning model choice with business risk priorities.

---

# Case 1: Personal Loan Prediction (Universal Bank)

## Objective

Classify whether a customer will accept a personal loan offer.

## Approach

- Compared k-Nearest Neighbors (kNN) and Classification Trees
- Identified optimal k using validation accuracy
- Evaluated models using 5-fold cross-validation

## Results

- Best kNN (k=7):
  - Validation Accuracy: 95.0%
  - Cross-validation Accuracy: 95.4%

- Classification Tree:
  - Validation Accuracy: 98.0%
  - Cross-validation Accuracy: 98.6%

## Decision

Classification Tree selected due to superior accuracy and interpretability.

**Business Impact:**
Enables targeted marketing and reduces unnecessary outreach costs.

---

# Case 2: Auction Competitiveness Prediction (eBay Dataset)

## Objective

Predict whether an auction will be competitive based on listing parameters.

## Key Insights from Decision Tree

Competitive auctions were strongly influenced by:

- **Opening Price**
- **Auction Duration**
- **Ending Day**

### Actionable Recommendations

- Set opening price below threshold (~$1.035) to increase competitiveness.
- Use auction durations ≤ 6 days.
- Avoid ending auctions on Sundays to improve competitive bidding likelihood.

## Model Refinement

Removed post-event variables (e.g., close price) to ensure predictions rely only on pre-listing information.

**Business Impact:**
Provides sellers with pre-launch guidance to maximize bidding competitiveness.

---

# Case 3: Industrial Alarm Intelligence (Drishya AI Lab Case)

## Business Problem

Frequent alarm floods and chattering at a SAGD plant were causing operational inefficiencies and safety risks.

## Objective

Predict alarm chattering behavior while minimizing false negatives (missed critical alarms).

## Models Developed

- kNN (Best k = 6)
  - Validation Accuracy: 89.7%
  - Test Accuracy: 79.35%

- Decision Tree
  - Training Accuracy: 96.37%
  - Validation Accuracy: 87.90%
  - Test Accuracy: 81.55%

## Risk Analysis

Although overall accuracy was strong, false negatives increased significantly in validation and test sets.

False Negative Rate increased from:
- 10.1% (Training)
- 26.3% (Validation)
- 19.8% (Test)

Given operational risk, minimizing missed chattering alarms was prioritized over reducing false positives.

## Alarm Tag Analysis

Identified and ranked alarm tags based on:

- Absolute number of chattering events
- Percentage of chattering occurrences per tag

Certain tags showed >55% chattering behavior, with some reaching near 100%.

**Business Impact:**

- Improved alarm prioritization
- Reduced operator overload
- Enhanced predictive maintenance strategy
- Supported risk-aware operational decision-making

---

## Key Skills Demonstrated

- k-Nearest Neighbors (kNN)
- Classification Trees
- Cross-Validation
- Feature Engineering
- Model Comparison & Selection
- Risk-Based Model Evaluation
- Business-Oriented Model Interpretation

---

## Core Takeaways

- Model selection must align with business cost structures (e.g., false negatives vs false positives).
- Interpretability matters for operational deployment.
- Feature refinement improves real-world usability.
- Predictive modeling applies consistently across finance, e-commerce, and industrial systems.

---

This project demonstrates applications in:

Banking Analytics | E-commerce Optimization | Industrial Predictive Maintenance | Risk Modeling | Decision Intelligence
