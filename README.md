# Security-log-pipeline

# Network Anomaly Detection using AI & Data Engineering

This project implements an end-to-end AI-driven intrusion detection pipeline using Databricks, PySpark, SQL, and Machine Learning.

## Project Overview
- Built Bronze-Silver-Gold data pipeline
- Processed large-scale IDS network traffic data
- Performed SQL-based analytics
- Applied ML models for attack detection

## Models Used
- Logistic Regression
- Random Forest (Best Model)
- Isolation Forest

## Results
- Accuracy: ~96%
- Precision: ~96%
- Recall: ~91%
- F1-score: ~93%

## Key Insights
- Packet rate, flow timing, and destination port are key indicators of attacks

## Project Structure
- notebooks/ → pipeline & ML code
- ml_results/ → model outputs

## Purpose
To convert raw network traffic into actionable security intelligence and detect malicious activity using AI.



This project implements an end-to-end AI-driven Security Log Data Pipeline using Databricks, PySpark, SQL, Delta Lake, and Machine Learning. The main purpose of the project is to convert raw, large-scale network traffic data into structured security intelligence and use machine learning to automatically detect malicious or abnormal activity.

Raw IDS network traffic files were ingested into Databricks and processed through a Bronze-Silver-Gold architecture. The Bronze layer stores raw ingested data, the Silver layer contains cleaned and structured data, and the Gold layer provides analytics-ready tables for security insights. SQL analytics were used to identify traffic patterns such as label distribution, protocol usage, and attack-port relationships.

Multiple machine learning models were implemented and compared, including Logistic Regression, Random Forest, and Isolation Forest. Random Forest was selected as the best-performing model, achieving approximately 96% accuracy, 96% attack precision, 91% attack recall, and 93% attack F1-score. Feature importance analysis showed that packet rate, flow timing, segment size, and destination port were key indicators of malicious traffic.

Overall, this project demonstrates how large-scale network logs can be transformed into actionable security intelligence for intrusion detection and cybersecurity decision-making.

Requirements
Databricks
pyspark
pandas
numpy
scikit-learn
matplotlib
seaborn
