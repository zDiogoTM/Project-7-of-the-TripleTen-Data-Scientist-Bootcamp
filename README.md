# 🚕 Taxi Data Analysis - Chicago
## 🎯 About the Project
Data analysis project combining SQL and Python to investigate taxi usage patterns in Chicago. The project explores ride data, company behavior, popular destinations, and tests hypotheses about factors influencing trip duration.
## 🔍 Business Context
Taxi companies need to understand:
Which regions have higher demand
How different companies compete in the market
External factors (such as weather) that affect operations
Optimization of routes and travel times
## 📂 Data Used
### Dataset 1: Rides by Company
project_sql_result_01.csv
trips_amount: number of rides per taxi company
Period: November 15-16, 2017
### Dataset 2: Destinations by Neighborhood
project_sql_result_04.csv
dropoff_location_name: Chicago neighborhoods where rides ended
average_trips: average number of trips completed per neighborhood
Period: November 2017
### Dataset 3: Hypothesis Testing
project_sql_result_07.csv
Specific Route: Loop → O'Hare International Airport
start_ts: ride start date/time
weather_conditions: weather conditions
duration_seconds: ride duration in seconds
## 🛠️ Methodology
### Phase 1: Data Extraction (SQL)
SQL queries for data aggregation and filtering
Integration of multiple tables
Temporal and geographical analysis
### Phase 2: Exploratory Analysis (Python)
Data import and validation
Data type verification
Identification of patterns and outliers
Analysis of the top 10 most popular neighborhoods
### Phase 3: Visualization
Chart: Taxi companies vs. number of rides
Chart: Top 10 neighborhoods by destination
Comparative analysis between companies
Geographical distribution of demand
### Phase 4: Statistical Hypothesis Testing
Hypothesis tested:
"The average duration of trips from the Loop to O'Hare Airport changes on rainy Saturdays"
Statistical approach:
Null Hypothesis (H₀): The average duration is equal on rainy and non-rainy Saturdays
Alternative Hypothesis (H₁): The average duration is different on rainy Saturdays
Test used: Student's t-test (or Mann-Whitney U, if non-parametric)
Significance level (α): 0.05
Decision criterion: p-value < α rejects H₀
## 💻 Technologies Used
SQL - data extraction and aggregation
Python 3.x
pandas - data manipulation
numpy - numerical operations
matplotlib / seaborn - visualization
scipy.stats - statistical tests
Jupyter Notebook - development
## 📈 Key Results
### Company Analysis
### Top 10 Neighborhoods
### Hypothesis Test
Test result:
p-value
Conclusion
Interpretation
### Business Insights
✓ [Insight 1 on demand patterns]
✓ [Insight 2 on weather impact]
✓ [Insight 3 on competition between companies]
✓ [Operational recommendations]
## 📊 Visualizations
The project includes visualizations for:
Distribution of rides by company
Ranking of most popular destination neighborhoods
Comparison of trip durations by weather condition
Temporal analysis of usage patterns
## 🚀 How to Run
### Prerequisites
Bash
pip install pandas numpy matplotlib seaborn scipy jupyter
### File structure
Plain Text
├── README.md
├── sprint_7_analise_taxi_chicago.ipynb
└── dados/
    ├── project_sql_result_01.csv
    ├── project_sql_result_04.csv
    └── project_sql_result_07.csv
### Running
Clone this repository
Place the CSV files in the dados/ folder
Open the Jupyter Notebook:
Bash
jupyter notebook sprint_7_analise_taxi_chicago.ipynb
## 💡 Demonstrated Competencies
This project demonstrates:
SQL: extraction and aggregation of relational data
Python: data analysis and manipulation
Statistics: hypothesis formulation and testing
Visualization: clear communication of insights
Critical thinking: interpretation of results
Business analysis: practical recommendations
## 🎓 Academic Context
Sprint 7 - TripleTen Data Science Bootcamp (2024)
This project integrates SQL and Python for comprehensive real-world data analysis, demonstrating an end-to-end data analysis pipeline.
Developed by: Diogo
GitHub: @zDiogoTM
