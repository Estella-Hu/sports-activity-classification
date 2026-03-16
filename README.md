# Sports Activity Classification with XGBoost and External Validation

## Project Overview
This project classifies sports activities using wearable-device data and evaluates whether the model generalizes to a fully unseen external dataset. The modeling pipeline combines data cleaning, feature engineering, multi-model comparison, and external validation to assess both predictive performance and real-world robustness.

## Motivation
Activity recognition is useful for health and fitness applications, but strong internal test performance alone is not enough. A model that performs well only on in-sample data may fail in practice when exposed to new users, devices, or behavior patterns. This project therefore emphasizes external validation as a core step in evaluating generalization.

## Methods
- Data cleaning and preprocessing
- Feature engineering
- Multi-model comparison across baseline and tree-based classifiers
- Tuned XGBoost multi-class classification
- External validation on unseen data
- Error analysis and feature interpretation

## Key Results
- The tuned XGBoost model achieved the strongest internal test performance among the candidate models.
- Performance declined moderately on the unseen external dataset, but overall accuracy and macro F1 remained solid.
- Error patterns were broadly consistent across internal and external testing, suggesting that the model captured meaningful activity-specific signals rather than overfitting to the training data.

## Selected Results

### Internal vs External Performance
![Internal vs External Performance](outputs/tables/Internal%20Testset%20Performance%20Comparison.png)

The tuned XGBoost model delivered the best overall internal test performance, outperforming non-boosting baselines in both accuracy and macro F1.

### External Validation Performance
![External Validation Performance](outputs/tables/External%20Validation%20Performance.png)

Performance dropped on the fully unseen external dataset, but the model still maintained solid overall results, indicating reasonable out-of-sample generalization.

### Feature Importance
![Feature Importance](outputs/tables/Feature%20Importance.png)

Speed-related and movement-efficiency features were the strongest signals, while route-shape and temporal features provided additional predictive value.

## My Contribution
- Participated in data cleaning and feature engineering
- Contributed to exploratory data analysis and model comparison
- Helped evaluate model performance on an unseen external dataset
- Interpreted results and summarized key findings for presentation

## Repository Structure
- `notebooks/`: EDA, modeling, and validation notebooks
- `outputs/tables/`: result tables and evaluation figures
- `docs/`: presentation materials
- `data/`: notes on dataset availability and sample data usage

## Team Attribution
This repository is a cleaned personal portfolio version of a team-based course project. The original project was completed collaboratively with my teammates. This version is organized to highlight the project workflow, evaluation results, and my specific contributions.

## Notes
This repository is intended for portfolio presentation rather than full reproduction of the original team development environment. The full raw dataset is not included in this repository.