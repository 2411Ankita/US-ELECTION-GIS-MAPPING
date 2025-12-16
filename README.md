# US-ELECTION-GIS-MAPPING
U.S. Congressional Election Analysis with GIS & Machine Learning (2012–2024)
Project Overview

This project analyzes and predicts voter turnout and election trends across U.S. congressional districts using GIS techniques and machine learning models. Due to incomplete and inconsistent data for recent elections, especially 2024, the project combines spatial analysis, supervised learning, and clustering to produce reliable turnout estimates.

The work focuses on integrating multi-year election data, addressing boundary changes, and handling missing information through data-driven modeling approaches.

Data Collection & Processing

Collected and processed 90%+ of U.S. election data (2012–2024) from multiple public and official sources

Integrated presidential, senate, and congressional district data

Addressed district boundary changes using areal interpolation with GIS

Cleaned and standardized demographic, turnout, and voting behavior features

Built ETL pipelines to align datasets across years with inconsistent schemas

Methodology
1. Exploratory & Predictive Analysis

Conducted both qualitative analysis (party trends, demographic influence) and quantitative prediction (turnout percentages)

Visualized turnout patterns using plots and GIS-based maps

2. Machine Learning Models

Logistic Regression

Initial baseline model

Performed poorly due to feature inconsistency and lack of 2024 labels

Random Forest

Improved accuracy over logistic regression for 2022 data

Captured nonlinear relationships

Suffered from overfitting and feature imbalance across years

KMeans Clustering (Final Approach)

Used for 2024 turnout prediction due to missing ground-truth data

Grouped districts by similar demographics and voting behavior

Tested k = 4 to 6 clusters

Predicted turnout using cluster-level historical averages

Results

Random Forest performed best for 2022 predictions but struggled with generalization

Clustering enabled reasonable 2024 turnout estimates despite missing data

Increasing cluster count improved differentiation between districts

GIS visualizations helped identify spatial and demographic voting patterns

Key Challenges

Lack of reliable 2024 turnout data

Inconsistent precinct and district boundaries across years

Missing or incomplete GIS datasets

Overfitting due to small or imbalanced samples

Feature selection and multicollinearity issues

What Worked Well

KMeans clustering as a robust solution for incomplete data

GIS-based areal interpolation to handle redistricting

Random Forest’s ability to model complex relationships

Data visualization for interpretability and insight generation

Future Improvements

Collect more consistent and complete 2024 datasets

Apply cross-validation and regularization to reduce overfitting

Improve feature engineering with interaction terms and composite indicators

Experiment with alternative clustering methods (DBSCAN, Agglomerative)

Incorporate external data such as campaign spending and political ads

Skills & Tools

Python

Geographic Information Systems (GIS)

Areal Interpolation

Machine Learning (Random Forest, KMeans)

ETL Pipelines

Data Visualization

Spatial & Demographic Analysis
