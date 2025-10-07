Big Data Analytics Project: Hospital Stay & Volume Analysis
Project Overview
This project utilizes Big Data technologies to analyze a comprehensive dataset of hospital admissions. The primary objective is to extract meaningful insights into operational trends, focusing specifically on patient volume over time and the factors that influence the Length of Stay (LOS).

Student: D . JESHWITHA
Roll No. / Academic Year: 2211CS010669 (S2-87) / 2025 - 2026

🛠 Technology Stack
Feature

Description

Value/Type

Platform

Distributed processing framework

Apache Spark (PySpark)

Data Volume

Total records analyzed

55,500 rows

Key Library

Used for DataFrame manipulation and aggregation

pyspark.sql.functions

📊 Data & Preprocessing
The analysis is based on a hospital admission dataset. Key steps in data preparation include:

Data Loading: Successfully loaded 55,500 records.

Temporal Transformation: Creation of the Admission_Year_Month field for time-series analysis.

Categorical Binning: Creation of the Age Group column (e.g., 21-40, 61-80) to facilitate demographic segmentation.

Sample Data Structure
Column Name

Data Type

Role in Analysis

Date of Admission

Date

Time-series base

Age

Integer

Used for binning

Age Group

String

Categorical variable

Length of Stay (Days)

Numeric

Target variable (LOS)

✅ Completed Analysis: Temporal Trends
Methodology
The PySpark DataFrames were grouped by Admission_Year_Month to calculate two crucial operational metrics: Monthly_Patients (volume) and Avg_Length_of_Stay.

Key Finding: Stable LOS vs. Fluctuating Volume
Initial analysis indicates a stable average Length of Stay (LOS) across the observed months, consistently falling between 15 and 16 days. However, the monthly patient volume shows distinct fluctuations, ranging from 686 to over 1000 patients.

Admission_Year_Month

Monthly_Patients

Avg_Length_of_Stay

2019-05

686

15.126

2019-07

957

15.928

2019-09

936

15.068

🔜 Future Work and Next Steps
The project is structured to proceed with deeper analytical phases to provide actionable operational insights.

1. Categorical Analysis
Goal: To determine if specific Age Groups are driving longer (or shorter) average lengths of stay.

Impact: Inform resource allocation for specialized care units catering to high-LOS demographics.

2. Bivariate Analysis
Goal: Investigate the relationship between LOS and billing data or other patient characteristics.

Impact: Identify drivers of cost efficiency and billing variations.

3. Predictive Modeling (Machine Learning)
Goal: Develop a Regression Model to accurately predict a patient's LOS based on their admission characteristics.

Impact: Improve hospital forecasting, bed management, and operational planning.
