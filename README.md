# Big-Data-Assignment
 Uber Fares Analysis using Python and Power BI
Overview
This project analyzes Uber ride fare patterns using Python (for data preparation and exploratory data analysis) and Power BI (for interactive dashboard visualization). The goal is to extract meaningful insights about ride pricing, time patterns, and user behavior from the Uber dataset.

📁 Project Structure

.
├── enhanced_uber_data.csv # Final cleaned and feature-engineered dataset
├── notebooks/
│ └── uber_fare_analysis.ipynb # Python Jupyter notebook for data cleaning and EDA
├── dashboard/
│ └── UberFaresDashboard.pbix # Power BI dashboard file (created in Power BI Desktop)
├── screenshots/
│ ├── data_loading.png # Screenshot of CSV loading into Power BI
│ ├── dashboard_view.png # Final dashboard screenshot
│ └── data_cleaning_steps.png # Image of Python cleaning process
└── README.md # Project documentation

📦 Dataset

Source: Sample Uber Fares Dataset

Download: Kaggle Link or sample file provided

Format: CSV

Key fields: pickup_datetime, fare_amount, trip_distance, passenger_count

🛠 Tools Used

Python 3.x

Jupyter Notebook

Pandas, Seaborn, Matplotlib

Power BI Desktop

📊 Features Engineered

The following new features were extracted from the pickup_datetime:

pickup_hour: hour of ride (0–23)

pickup_day: calendar day

pickup_month: month number

pickup_dayofweek: day of week (0 = Monday)

pickup_day_name: full name of weekday

is_peak: binary (1 if hour is in peak range, 0 otherwise)

is_weekend: binary (1 for Saturday/Sunday)

🧪 Data Cleaning Summary

Removed rows with missing fare_amount or pickup_datetime

Filtered out fares ≤ 0 and above $200

Converted pickup_datetime to datetime object

Exported cleaned data to enhanced_uber_data.csv for Power BI

📈 Dashboard Highlights

Created using Power BI Desktop, the dashboard includes:

Histogram: Fare Amount Distribution

Line Chart: Average Fare by Hour

Column Chart: Rides by Day of Week

Donut Chart: Peak vs Off-Peak Rides

Area Chart: Monthly Fare Trends

Slicers: Filter by hour, weekday, peak/off-peak

📌 How to Run This Project

Clone or download the repository

Open the notebook in Jupyter to explore and clean the data

Open enhanced_uber_data.csv in Power BI

Customize visuals or publish to Power BI Service

📄 License

This project is licensed under the MIT License. You are free to use and adapt it.

🙌 Credits

Dataset:  Kaggle

Developed by: [Joy B]

Tools: Python, Jupyter, Power BI
