# Healthcare-Analytics-Dashboard
Build a data-driven dashboard to monitor hospital performance, patient admissions, treatment costs, and doctor efficiency.
📅 Day 12 of My 15-Day Data & Business Analysis Challenge

This project focuses on analyzing hospital and patient data to uncover insights into healthcare performance, treatment costs, and patient satisfaction using Power BI. The dashboard provides a holistic view of hospital operations — from patient admissions to cost efficiency and readmission trends.

📘 Project Overview

In today’s data-driven healthcare systems, it’s crucial to track operational performance, patient outcomes, and cost efficiency effectively.

This dashboard was built using Power BI and a hospital dataset (Kaggle) to visualize key metrics like Total Patients, Treatment Cost, Average Stay, Readmission Rate, and Satisfaction Levels.

The aim is to help healthcare administrators and analysts make informed decisions that improve patient care and resource allocation.

🧩 Dataset Description

Dataset Columns:

Patient_ID, Age, Gender, Condition, Procedure, Cost,
Length_of_Stay, Readmission, Outcome, Satisfaction,
Total Patients, Total Treatment Cost,
Average Cost per Patient, Average Length of Stay, Readmission Rate


Rows: Each record represents a unique patient visit.

Period: Simulated dataset representing hospital admissions and treatments.

🛠 Tools Used

Power BI – Dashboard creation and visualization

Excel / CSV – Data storage and initial cleaning

DAX – Custom measures and calculations

Power Query – Data transformation and relationship modeling

🧮 DAX Measures Used
Total Patients = DISTINCTCOUNT('hospital data analysis'[Patient_ID])
Total Treatment Cost = SUM('hospital data analysis'[Cost])
Average Cost per Patient = DIVIDE([Total Treatment Cost], [Total Patients], 0)
Average Length of Stay = AVERAGE('hospital data analysis'[Length_of_Stay])
Readmission Count = CALCULATE(COUNTROWS('hospital data analysis'), 'hospital data analysis'[Readmission] = "Yes")
Readmission Rate = DIVIDE([Readmission Count], [Total Patients], 0)
Average Satisfaction = AVERAGE('hospital data analysis'[Satisfaction])

📊 Dashboard Features
1️⃣ Overview Page

KPIs: Total Patients, Treatment Cost, Avg Cost per Patient, Avg Length of Stay, Readmission Rate

Trendline: Treatment cost changes over time

2️⃣ Condition & Procedure Analysis

Bar chart: Treatment cost by medical condition

Column chart: Average stay vs cost by procedure

3️⃣ Demographics & Outcomes

Pie chart: Gender distribution

Age group insights for cost and readmission rate

Table: Procedure, Outcome, Satisfaction, Readmission

4️⃣ Interactive Filters

Slicers for Gender, Condition, Outcome, Procedure

💡 Key Insights

Cardiology and Neurology departments have the highest cost and longer stay durations.

Elderly patients (60+) face higher readmission rates and lower satisfaction.

Shorter hospital stays correlate with higher satisfaction and fewer readmissions.

Cost optimization opportunities found across certain procedures.

Balanced performance across departments indicates strong management and follow-up care.

✅ Conclusion & Takeaway

This dashboard transforms raw hospital data into meaningful healthcare insights.
By visualizing patient journeys, cost efficiency, and satisfaction trends, it empowers decision-makers to enhance care quality, reduce costs, and improve overall hospital performance.

📂 Project Files

Power BI File (.pbix) – Interactive dashboard

Dataset (.csv) – Hospital/Patient Data

DAX Formulas (.txt) – All custom measures

👨‍💻 Author

Khawaja Hizbullah
Data & Business Analyst
📍 Pakistan | ✉️ khawajahizbullah@gmail.com

🔗 LinkedIn
 | GitHub

⭐ Acknowledgment

Dataset sourced and adapted from Kaggle’s Hospital/Patient Analytics dataset for educational and analytical practice.
