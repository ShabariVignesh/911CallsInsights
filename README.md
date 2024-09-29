# 911CallsInsights
This project analyzes 911 emergency call data to uncover patterns and trends that can improve resource allocation, response times, and emergency management. Using data from Kaggle, the analysis focuses on call frequency, geographical distribution, and temporal trends to provide actionable insights for optimizing emergency services.

## Project Objectives
- Analyze the frequency and types of emergency calls.
- Identify temporal patterns in emergency calls (daily, weekly, monthly trends).
- Examine geographical distribution of calls.
- Investigate correlations between call types and specific times or locations.

## Expected Outcomes
The analysis aims to provide insights that help emergency services optimize resource allocation, improve response times, and enhance emergency management strategies.

## Data Source
The dataset is sourced from [Kaggle](https://www.kaggle.com/mchirico/montcoalert) and includes information on 911 emergency calls, such as timestamps, locations, and call descriptions.

## Data Cleaning and Processing
- **Handling Missing Values**: Some columns (e.g., zip, twp, addr) had minimal missing data, which was not filled due to its minimal impact.
- **Data Type Conversion**: The `timeStamp` column was converted to DateTime format for time-based analysis.
- **Feature Extraction**: Additional features were derived from the `timeStamp` column, including Hour, Month, Day of Week, and Date. A new column, `Reasons`, was created by extracting the emergency type (EMS, Fire, Traffic) from the `title` column.

## Data Analysis
Analysis was conducted using Python libraries like Pandas, Seaborn, and Matplotlib in Google Colab. Key analysis areas include:
- **Top Zip Codes and Townships for 911 Calls**: Identifying areas with the highest volume of emergency calls.
- **Common Reasons for 911 Calls**: EMS (Emergency Medical Services) was found to be the most common reason.
- **Time-Based Trends**: Grouping data by hour, month, and day of the week to reveal peak times for emergency calls.

## Insights
- **Zip Codes and Townships**: Certain areas experience a higher volume of emergency calls.
- **Common Call Reasons**: EMS calls are the most frequent, followed by Fire and Traffic-related emergencies.
- **Temporal Patterns**: Certain times of day and days of the week experience more emergency calls, which can guide resource allocation.

## Tools Used
- **Python**: For data analysis and visualization (Pandas, Matplotlib, Seaborn).
- **Google Colab**: The platform used for executing the analysis.
- **Excel**: For initial data cleaning and processing.

## Recommendations
Based on the analysis, emergency service departments can:
- Optimize staffing levels based on high-call volume times and locations.
- Improve resource allocation in areas with frequent emergencies.
- Develop targeted prevention strategies and public safety education programs.

## Conclusion
This project provides valuable insights into 911 emergency call patterns and trends, with the potential to enhance resource management and improve response times for emergency services.

