# Ghost Job Detection & Fraud Monitoring
Detecting fraudulent (“ghost”) job postings using feature engineering, a Random Forest machine learning model, and an interactive Power BI dashboard.

## Project Objective

Many job portals contain fake or misleading job posts created to collect data, advertise, or scam applicants.
This project identifies such postings by building a Ghost Score based on suspicious patterns and training a machine learning model to classify fraud risk.

## Dataset

This project uses the Fake Job Postings Dataset available on Kaggle:

Dataset Link:
https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction

The dataset is not included in this repository due to size limitations.

### Steps to use the dataset
Download the dataset from the above link
Place the CSV file inside a folder named data in this project
Run the notebook/script to reproduce the results

## Project Workflow
* Data Cleaning and preprocessing of raw job posting data
* Feature Engineering to identify fraud indicators (missing salary, keywords, company info, etc.)
* Creation of a custom Ghost Score to quantify fraud risk
* Training a Random Forest model to classify job posts
* Exploratory Data Analysis (EDA) to discover major fraud drivers
* Building an interactive Power BI Dashboard for fraud monitoring

## Key Features Engineered
* Salary Missing indicatorCompany Profile Missing indicator
* Suspicious Keywords count (e.g., earn money, quick cash)
* Description Length
* Employment Type handling
* Ghost Score calculation
* Risk Level categorization (Safe, Suspicious, Likely Ghost)

## Machine Learning Model
* Algorithm: Random Forest Classifier
* Target Variable: Fraudulent Job Post (0 / 1)
* Output: Fraud probability and risk classification

## Power BI Dashboard
The dashboard visualizes:
* Ghost Score Distribution
* Fraud Rate by Risk Level
* Impact of Missing Salary on Fraud
* Employment Type vs Fraud
* Risk Rate by Industry

## Repository Structure
```
ghost-job-detection-fraud-monitoring/│
├── notebook/
│   └── ghost_job_detection.ipynb
│
├── powerbi/
│   └── ghost_job_dashboard.pbix
│
├── images/
│   ├── dashboard.png
│   ├── ghost_score_chart.png
│   └── fraud_by_risk.png
│
├── INSIGHT.md
│
└── README.md
```


## Tools & Technologies Used
* Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
* Power BI (DAX, Data Modeling, Visualization)
* Jupyter Notebook

## Results
The project successfully identifies patterns commonly found in ghost job postings and classifies them into risk categories, helping users and platforms detect fraudulent listings effectively.

## Author
Nikita Arora
