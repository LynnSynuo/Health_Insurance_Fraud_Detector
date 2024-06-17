# Health_Insurance_Fraud_Detector

# Project Description
Health insurance fraud is a significant challenge facing Medicare, a federal health insurance program. \
As the Fraud Detection and Prevention Unit, our mission is to assist Medicare in identifying and preventing potential fraudulent claims.

We have proposed two strategic approaches to address this issue:
- Identify fraudulent claims: By detecting individual fraudulent claims, we can uncover patterns that may indicate broader systemic issues.
- Identify false healthcare provider: By scrutinizing healthcare providers, we can expose those who engage in fraudulent practices.

Detecting a single fraudulent claim can often reveal larger, underlying patterns of fraud, \
helping us protect Medicare's integrity and ensure its resources are used appropriately.

# Benchmark
- Benchmark 1: Rely on domain experts to manually review claims, ~0.00%
- Benchmark 2: Claim Audits Team , random or target, vary 20%-40%

# Metrics to Evaluate the Effectiveness of the Model
- False Positive: Denial of Insurance Benefits for Legitimate Claims.
Business Impact: Degrade the insurance companies’ reputation and undermine customer trust.

- False Negative: Authorization of Insurance Benefits for Fraudulent Claims.
Business Impact: Lead to significant monetary losses for insurance companies.

- Fβ Score: Keep a balance between business interests and the company's reputation, with the exact beta value determined by the company's economic situation and strategic objectives.



# Phases of a Medical Bill
![Phases_of_a_medical-bill](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/dd0591c5-c8f3-4720-9b24-ea2b638a9047)

# How the Fraud Detector Works? 
![Medical Provider Fraud Detector_2023 12 15 updated (1)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/785a5171-9ff7-4839-b296-b50ca69d428c)

# Data Source
- Data source: https://www.kaggle.com/datasets/rohitrox/healthcare-provider-fraud-detection-analysis/ 
- Data from Medicare, a federal health insurance program in the United States
- Historical claim data from 2009
- Multiple datasets


# Data Structure
![DB schema_2023 12 08 updated](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/9742dade-8258-4131-9d1d-e0b1c0eb75d0)


# Claims Get Processed Each Week_Inpatient
- Claim processing duration: 5.5 days in average
- Frequency of running model: Weekly
- 764 claims are processed each week in average

![download](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/49cad5ed-1528-43ee-a34b-2862552f0d5f)

# Split Data In Progressive Manner
- Split the data into training and testing sets in a progressive manner 
- Train & predict with different data at each step

![Medical Provider Fraud Detector_2023 12 15 updated (2)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/71338fc9-689e-45f4-9779-169edfe9e650)

# Model Performance Overtime

![Medical Provider Fraud Detector_2023 12 15 updated (3)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/c8acbd74-2e33-4f3b-a044-79fdb766f9f7)

# Claims Get Processed Each Day_Outpatient
- Claim processing duration: 1.4 days in average
- Frequency of running model: Daily
- 1,415 claims are processed each day in average

![download (1)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/71c4d7be-998e-41c0-a9e2-7ee53c2a1b89)

# Model Performance Overtime

![u](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/0a8122f9-5507-436b-915d-8084a0570143)

# License
