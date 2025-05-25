
# Waze User Churn Analysis

This project is part of the **Google Advanced Data Analytics** course and focuses on analyzing user churn and retention rates for the Waze navigation app. Through exploratory data analysis, statistical modeling, and business strategy development, the project aims to identify key drivers of churn and propose actionable retention strategies.

---

## Background on the Waze Scenario
Waze’s free navigation app makes it easier for drivers around the world to get to where they want to go. Waze’s community of map editors, beta testers, translators, partners, and users helps make each drive better and safer. Waze partners with cities, transportation authorities, broadcasters, businesses, and first responders to help as many people as possible travel more efficiently and safely.

This project will involve collaboration with Waze teammates to analyze and interpret data, generate valuable insights, and help leadership make informed business decisions. The team is about to start a new project to help prevent user churn on the Waze app. Churn quantifies the number of users who have uninstalled the Waze app or stopped using the app. This project focuses on monthly user churn. In my role, I will analyze user data and develop a machine learning model that predicts user churn.

This project is part of a larger effort at Waze to increase growth. Typically, high retention rates indicate satisfied users who repeatedly use the Waze app over time. Developing a churn prediction model will help prevent churn, improve user retention, and grow Waze’s business. An accurate model can also help identify specific factors that contribute to churn and answer questions such as:

- Who are the users most likely to churn?
- Why do users churn?
- When do users churn?

For example, if Waze can identify a segment of users who are at high risk of churning, Waze can proactively engage these users with special offers to try and retain them. Otherwise, Waze may simply lose these users without knowing why.

My insights will help Waze leadership optimize the company’s retention strategy, enhance user experience, and make data-driven decisions about product development.

---

## Project Overview

User churn — when users stop using an app — is a critical metric for any tech product. Understanding the factors influencing churn helps businesses improve user experience, increase customer lifetime value, and reduce acquisition costs.

In this analysis, Waze user behavior data was explored to:

- Identify patterns and trends linked to churn
- Develop a predictive model to forecast user churn
- Recommend targeted business interventions to improve retention

---

## Key Insights, Conclusions & Recommendations

The analysis reveals that approximately 18% of users churn while the majority (82%) are retained, with churned users typically driving longer distances on fewer days. Frequent app usage strongly correlates with retention, while higher average kilometers per driving day relates to increased churn risk. User device type showed no statistically significant impact on driving behavior, though further behavioral analysis is recommended.

Initial predictive modeling using binomial logistic regression demonstrated limited ability to identify churned users, with low recall (only 9%) despite moderate precision. More advanced machine learning models, including random forests and XGBoost, improved predictive performance, nearly doubling recall to 17% while maintaining similar accuracy and precision. These ensemble tree-based models benefited significantly from engineered features derived from the data, though they remain less interpretable than simpler models.

Despite these advances, the modeling underscores a critical need for more detailed, granular data—such as drive-level information and user interactions with the app—to further enhance churn prediction accuracy. The Waze team recommends ongoing data enrichment and iterative model development to better understand churn drivers and optimize user retention strategies.

---

## Repository Structure

```plaintext
waze-user-churn-analysis/
├── Notebooks/           # Jupyter notebooks for data exploration, cleaning, and modeling
│   ├── 1 - Data Inspection and Preliminary Analysis.ipynb
│   ├── 2 - EDA.ipynb
│   ├── 3 - Hypothesis Testing.ipynb
│   ├── 4 - Regression Modeling.ipynb
│   └── 5 - Machine Learning.ipynb
├── Docs/                # Supporting documentation such as proposals and executive summaries
│   ├── Waze Project Proposal.pdf
│   ├── PACE Strategy Document.pdf
│   ├── Preliminary Data Summary.pdf
│   ├── Executive Summary - Data Inspection and Preliminary Analysis.pdf
│   ├── Executive Summary - EDA.pdf
│   ├── Executive Summary - Hypothesis Testing.pdf
│   ├── Executive Summary - Regression Modeling.pdf
│   └── Executive Summary - Machine Learning Modeling.pdf
├── README.md            # This file
