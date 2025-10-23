
# Project Success Prediction Analytics

## Overview

This repository contains a synthetic dataset and exploratory data analysis (EDA) notebook designed to help you practice and showcase skills relevant to Business Analysts, Program Managers, and Data Analysts. The project simulates factors influencing the success of various projects and demonstrates how to use data analytics techniques to gain insights and build predictive models.

The repository includes:

- **data/synthetic_project_data.csv**: A synthetic dataset with 1,000 project records and 13 features (12 input features and 1 target).
- **analysis.ipynb**: A Jupyter Notebook that performs EDA, visualizations, and trains a classification model to predict project success.
- **requirements.txt**: A list of Python package dependencies required to run the notebook.

## Synthetic Dataset

The dataset is generated programmatically and does not contain real-world data. Each project record includes attributes such as project type, region, industry, budget, team size, duration, stakeholder engagement, risk score, complexity score, number of issues encountered, prior success rate, and the binary target `success`. The target variable indicates whether a project is considered successful based on a combination of factors.

| Column | Description |
| --- | --- |
| `project_id` | Unique identifier for each project |
| `project_type` | Category of the project (e.g., Software, Infrastructure, Marketing, Research, HR) |
| `region` | Geographic region where the project is executed |
| `industry` | Industry sector associated with the project |
| `budget` | Total budget allocated to the project (USD) |
| `team_size` | Number of team members assigned to the project |
| `duration_months` | Duration of the project in months |
| `stakeholder_engagement_score` | Score representing stakeholder engagement on a scale of 0-100 |
| `risk_score` | Risk assessment score on a scale of 0-100 |
| `complexity_score` | Complexity assessment score on a scale of 0-100 |
| `num_issues` | Number of issues encountered during the project |
| `prior_success_rate` | Historical success rate for similar projects (0-1) |
| `success` | Target variable indicating project success (1=successful, 0=unsuccessful) |

## Usage

To explore and run the analysis notebook locally, follow these steps:

1. **Clone the repository:**

```bash
git clone <repository-url>
cd project-success-prediction-analytics
```

2. **Create a virtual environment (optional but recommended):**

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scriptsctivate`
```

3. **Install dependencies:**

```bash
pip install -r requirements.txt
```

4. **Launch Jupyter Notebook:**

```bash
jupyter notebook analysis.ipynb
```

5. **Explore the notebook:**

The notebook includes sections for loading the data, descriptive statistics, visualizations, and model training. Feel free to modify or extend the analysis for your own learning or presentation.

## Extending the Project

To increase the difficulty and showcase additional skills, consider adding the following enhancements:

- Perform feature engineering (e.g., creating interaction terms or aggregate metrics) to improve model performance.
- Evaluate different machine learning algorithms (e.g., logistic regression, gradient boosting) and compare their results.
- Implement cross-validation and hyperparameter tuning using `GridSearchCV` or `RandomizedSearchCV`.
- Use SHAP or permutation importance to interpret model results and understand the impact of each feature.
- Deploy the model using a REST API framework such as Flask or FastAPI and integrate it into a simple dashboard.

## License

This project is released under the MIT License and may be used freely for educational purposes.
