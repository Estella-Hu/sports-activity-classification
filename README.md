# Sports Activity Classification with XGBoost and External Validation

## Project Overview
This project classifies sports activities using wearable-device data and evaluates whether the model generalizes to a fully unseen external dataset.

## Motivation
Activity recognition is useful for health and fitness applications, but strong internal performance alone is not enough. This project focuses on external validation to assess real-world generalization.

## Methods
- Data cleaning and preprocessing
- Feature engineering
- XGBoost multi-class classification
- External validation on unseen data
- Error analysis and feature interpretation

## Key Results
- The model achieved strong internal performance and maintained solid results on an unseen external dataset.
- Major activity classes showed limited performance drop during external validation.
- Error patterns were broadly consistent across internal and external testing.

## My Contribution
- Participated in data cleaning and feature engineering
- Contributed to EDA and model comparison
- Helped evaluate model performance on an unseen external dataset
- Interpreted results and summarized key findings for presentation

## Repository Structure
- `notebooks/`: EDA, modeling, and validation notebooks
- `outputs/figures/`: visualizations and evaluation charts
- `outputs/tables/`: model performance summaries
- `docs/`: presentation materials

## Team Attribution
This repository is a cleaned personal portfolio version of a team project. The original work was completed collaboratively with my teammates, and this version is organized to highlight the project workflow, results, and my specific contributions.

## Selected Results

### Internal vs External Performance
![Internal vs External Performance](outputs/tables/Internal%20Testset%20Performance%20Comparison.png)

### External Validation Performance
![External Validation Performance](outputs/tables/External%20Validation%20Performance.png)

### Feature Importance
![Feature Importance](outputs/tables/Feature%20Importance.png)