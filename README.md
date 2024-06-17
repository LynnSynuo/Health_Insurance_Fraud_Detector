# Health_Insurance_Fraud_Detector

# Project Description
Health insurance fraud is a significant challenge facing Medicare, a federal health insurance program. As the Fraud Detection and Prevention Unit, our mission is to assist Medicare in identifying and preventing potential fraudulent claims.

# What is the problem you would like to solve? Why is it important?
- Healthcare Fraud is one of the major problems in the US Healthcare System, leading to tens of billions of dollars lost each year.  

- Insurance Agencies like Medicare, Medicaid, and other agencies have to spend more money, and to incur financial losses, they have to decide to increase the insurance premium amount. Eventually, the healthcare system is becoming more and more expensive for everyone.

- Not only is financial loss a major concern, but fraud can also lead to unnecessary procedures, inappropriate medications, and even over-treatment, putting patients at risk. 

# Business Value of the Solution
- Goal: Detect as many fraud claims as possible

- The average cost of $1000 per claim reimbursement

- Every 1% increase in detection rate can save hundreds of millions nationwide



# Benchmark
- Benchmark 1: Rely on domain experts to manually review claims, ~0.00%
- Benchmark 2: Claim Audits Team, random or target, vary 20%-40%

# Metrics to Evaluate the Effectiveness of the Model
- False Positive: Denial of Insurance Benefits for Legitimate Claims.
Business Impact: Degrade the insurance companies’ reputation and undermine customer trust.

- False Negative: Authorization of Insurance Benefits for Fraudulent Claims.
Business Impact: Leads to significant monetary losses for insurance companies.

- Fβ Score: Balance business interests and the company's reputation, with the exact beta value determined by the company's economic situation and strategic objectives.\
![F-beta](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/29bc7671-97bb-4b67-9941-51d06db1e96b)



# Data Source
- Data source: https://www.kaggle.com/datasets/rohitrox/healthcare-provider-fraud-detection-analysis/ 
- Data from Medicare, a federal health insurance program in the United States
- Historical claim data from 2009
- Multiple datasets

# Data Structure
![DB schema_2023 12 08 updated](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/9742dade-8258-4131-9d1d-e0b1c0eb75d0)


# Input and Output Data
## Phases of a Medical Bill

![Phases_of_a_medical-bill](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/dd0591c5-c8f3-4720-9b24-ea2b638a9047)
## Input data
- Internal data of payer
  - EHR of beneficiaries
- Claim transferred from medical provider to payer
  - Inpatient
  - Outpatient

## Output data
- Medical Provider is fraudulent or not


# What will be the output feature?
![Medical Provider Fraud Detector_2023 12 15 updated (1)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/785a5171-9ff7-4839-b296-b50ca69d428c)

# Strategy
We have proposed two strategic approaches to address this issue:
- Identify fraudulent claims: By detecting individual fraudulent claims, we can uncover patterns that may indicate broader systemic issues.
- Identify false healthcare providers: By scrutinizing healthcare providers, we can expose those who engage in fraudulent practices.

Detecting a single fraudulent claim can often reveal larger, underlying patterns of fraud, helping us protect Medicare's integrity and ensure its resources are used appropriately.

# Suggestions for Running Models
## Process Inpatient Claims Every Week
- Inpatient Claim processing duration: 5.5 days on average
- Frequency of running model: Weekly
- 764 claims are processed each week on average

![download](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/49cad5ed-1528-43ee-a34b-2862552f0d5f)

### Split Data In Progressive Manner
- Split the data into training and testing sets in a progressive manner 
- Train & predict with different data at each step

![Medical Provider Fraud Detector_2023 12 15 updated (2)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/71338fc9-689e-45f4-9779-169edfe9e650)

### Inpatient Model Performance Overtime

![Medical Provider Fraud Detector_2023 12 15 updated (3)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/c8acbd74-2e33-4f3b-a044-79fdb766f9f7)

## Process Outpatient Claims Every Day
- Outpatient Claim processing duration: 1.4 days on average
- Frequency of running model: Daily
- 1,415 claims are processed each day on average

![download (1)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/71c4d7be-998e-41c0-a9e2-7ee53c2a1b89)

### Outpatient Model Performance Overtime

![u](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/0a8122f9-5507-436b-915d-8084a0570143)

