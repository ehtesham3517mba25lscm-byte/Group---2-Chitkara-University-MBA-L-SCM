Maritime Bottleneck Identification & Predictive Analysis
This project provides an automated, end-to-end data science pipeline designed to identify, analyze, and predict regional maritime port bottlenecks. By leveraging historical port stay data, this framework transforms raw logs into actionable intelligence, helping stakeholders understand how vessel characteristics and regional factors drive global supply chain delays.

🛠 Project Purpose
The core objective is to answer: Which economies are experiencing the highest median port stay times for specific vessel types, and why?

This project moves beyond descriptive reporting by integrating:

Exploratory Data Analysis (EDA): Visual identification of regional bottlenecks.

Predictive Machine Learning: Forecasting wait times for future vessel arrivals.

Statistical Validation: Mathematical proof (T-tests/Correlation) ensuring that reported delays are structurally significant and not due to random chance.

🚀 Workflow Overview
1. Data Processing
Cleaning: Standardization of raw maritime logs.

Feature Engineering: Extraction of temporal variables (Year, Semester) and categorical encoding of vessel types/regions to prepare data for modeling.

2. Diagnostic Analysis (EDA)
Generates a Heatmap to visualize the intersection of regions and ship types. This acts as a "bottleneck detector," pinpointing where operational efficiency is lowest.

3. Predictive Modeling
Utilizes a RandomForestRegressor within a Pipeline.

Learns complex, non-linear relationships between vessel metrics (Avg_Age, Avg_Size_GT, Avg_TEU) and Median_Port_Time to predict future congestion.

4. Statistical Validation
Feature Importance: Identifies the primary drivers (e.g., vessel size vs. age) causing delays.

Significance Testing: Employs T-tests and P-value analysis to provide a rigorous, academic foundation for all findings presented.

📋 Requirements
To run this analysis, ensure you have the following libraries installed:

Bash
pip install pandas scikit-learn matplotlib seaborn scipy
📈 Key Research Contributions
Identification: Visual detection of regional bottlenecks.

Optimization: Insights into whether delays are caused by vessel-region mismatches or port infrastructure.

Credibility: Empirically grounded results backed by statistical significance (P < 0.05).
