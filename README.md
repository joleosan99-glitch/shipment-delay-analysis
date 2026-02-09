🚢 Shipment Delay Analysis – Case Study
📌 Project Overview
This project analyzes shipment delays in container shipping operations using historical vessel movement and port event data.
The objective is to identify delay patterns, on-time performance, and ships with the highest delay risk, then present insights through a Power BI dashboard.

This case study demonstrates skills in:
• Data cleaning & validation
• SQL & Pandas-based analysis
• KPI design
• Business-focused data storytelling
• Dashboard presentation

📊 Data Source
The dataset is sourced from Kaggle – Container Ship Data Collection, containing over 800,000 AIS records, including:
• Vessel positions (latitude, longitude)
• Speed and heading
• Departure & arrival ports
• Scheduled vs actual arrival times (ETA vs ATA)

Due to data size constraints, the full dataset (~26GB) is not uploaded to this repository.

🧹 Data Cleaning & Preparation
Data preparation was performed using SQLite (via DBeaver) and Pandas, with the following steps:
• Standardized blank values to NULL
• Converted date and time columns to proper datetime format
• Validated NULLs, blanks, and zero values
• Created a cleaned shipment dataset for analysis
• Calculated shipment delay in minutes (ETA vs ATA)
• Filtered invalid or incomplete shipment records

Data quality checks were conducted using both SQL queries and Pandas validation scripts.

📐 Key Metrics
The analysis focuses on the following KPIs:
• Total Shipments
• On-Time Shipment Rate
• Average Delay (Minutes)
• Delayed Shipments by Vessel
• Delay Distribution by Route (Port to Port)

📈 Dashboard
The final analysis is presented in a Power BI dashboard, exported as PDF:
📄 Dashboard File
dashboard/Dashboard_Shipment_Delay_Analysis_Case_Study.pdf

The dashboard includes:
• Overall on-time performance
• Average delay by ship
• Top delayed ships
• Port-to-port shipment overview
• Key business insights summary

🔍 Key Insights
• Shipment delays are concentrated on a small number of vessels, rather than evenly distributed.
• Certain ships consistently show higher average delay minutes, indicating potential operational or scheduling issues.
• Despite a large dataset size, the number of distinct ships and routes is limited, resulting in repeated patterns.

Focusing on high-delay vessels provides more actionable insights than route-level aggregation alone.

⚠️ Data Availability Note
To keep this repository lightweight and recruiter-friendly:
• Full raw and cleaned datasets are excluded
• SQL database files are not uploaded due to size
• All analytical steps and assumptions are documented in this README

🛠 Tools & Technologies
• SQL (SQLite)
• DBeaver
• Python (Pandas)
• Power BI
• GitHub

👤 Author
Johnny Saputra
Data Analyst Portfolio Project

⭐ Notes for Recruiters

This project emphasizes analytical thinking, data validation, and insight communication, rather than dataset size or visualization complexity.
