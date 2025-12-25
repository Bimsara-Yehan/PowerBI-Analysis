🏭 Manufacturing Performance & Quality Control Dashboard
📋 Project Overview
This project features a multi-page Power BI dashboard designed to provide actionable insights for manufacturing plant managers. The dashboard analyzes over 3,000 production records to identify correlations between maintenance schedules, worker productivity, and final product quality.
Key Objective: To transform raw manufacturing logs into a strategic tool for reducing downtime and optimizing production costs.

🚀 Live Demo Features
Executive Overview: Real-time KPI monitoring with conditional formatting alerts.
Operational Deep-Dive: Analysis of machine downtime vs. delivery delays using scatter plots and trend lines.
Financial Analytics: Unit cost breakdown via Decomposition Trees and Quadrant Analysis to identify high-cost/low-quality production runs.
Time-Series Animation: A Play Axis implementation visualizing the trade-off between Production Volume and Quality Score over a 12-month period.

🛠️ Technical Implementation
1. Data Modeling
Implemented a Star Schema to ensure optimal performance.
Fact Table: fact_manufacturing (3,240 rows).
Dimension Tables: Dim_Date (Calendar table for time-intelligence).

2. Advanced DAX Measures
Selected key measures developed for this project:
Critical Defects: Filters the 84% baseline defect rate to highlight only high-severity quality failures (Quality Score < 60).
Unit Cost: DIVIDE([Total Production Cost], [Total Production Volume]) to normalize spending across varying production scales.
Efficiency Ratio: Calculated using EnergyEfficiency and WorkerProductivity metrics to gauge operational health.

3. UI/UX Design
Custom Navigation: Built a vertical sidebar using the Page Navigator for an application-style experience.
Visual Hierarchy: Used rounded containers with soft drop-shadows to separate data "zones" and reduce cognitive load.
Color Theory: Employed a "Dark Mode" sidebar for contrast against "Light Mode" data cards to guide user focus toward primary KPIs.

📊 Dataset Insights
The dataset used (Source: Kaggle Manufacturing Defect Dataset) revealed:
An average defect rate of ~2.8% per run.
A strong correlation between Maintenance Hours and Downtime Percentage, allowing for predictive maintenance scheduling.
High sensitivity in DefectStatus, requiring custom filtering logic to identify truly non-conforming products.


🧠 Skills Applied
Data Cleaning & Transformation (Power Query / M)
Relational Data Modeling
Advanced DAX
UI/UX for Business Intelligence
