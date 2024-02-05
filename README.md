# Health_Insurance_Fraud_Detector

# Project Description
Health insurance fraud is one of the biggest problem facing medicare\
We work as a fraud team in Medicare, a federal health insurance program

We proposed two directions to address this problem:
- Identify fraudulent claims
- Identify false healthcare provider

Discovering a single fraudulent claim could indicate a pattern or a systemic issue

# Case of Healthcare Fraud
“The majority of fraud cases are schemes perpetrated by highly sophisticated organizations, not hospitals or physicians who may make a billing error or two,” Stewart said. 
“For example, criminal organizations may buy health data on the dark web, pose as clinicians, and then submit fake health insurance claims using the data.”
                                                                                                                            - Blue Cross Blue Shield of Massachusetts

Earlier this year, a Michigan doctor was sentenced to prison for defrauding health insurers out of $250 million by billing for unnecessary spinal injections as part of an opioid distribution scheme. Over a five-year period, the physician billed Medicare for these lucrative injections more than any other provider in the nation, giving opioid prescriptions to patients who would receive the medically needless shots. 
                                                                                                                            - Definitive Healthcare
# Common Types of Healthcare Fraud
- Fraud Committed by Medical Providers

Double billing: Submitting multiple claims for the same service\
Phantom billing: Billing for a service visit or supplies the patient never received \
Unbundling: Submitting multiple bills for the same service \
Upcoding: Billing for a more expensive service than the patient actually received

- Fraud Committed by Patients and Other Individuals

Bogus marketing: Convincing people to provide their health insurance identification number and other personal information to bill for non-rendered services, steal their identity, or enroll them in a fake benefit plan\
Identity theft/identity swapping: Using another person’s health insurance or allowing another person to use your insurance\
Impersonating a healthcare professional: Providing or billing for health services or equipment without a license

- Fraud Involving Prescriptions

Forgery: Creating or using forged prescriptions\
Diversion: Diverting legal prescriptions for illegal uses, such as selling your prescription medication\
Doctor shopping: Visiting multiple providers to get prescriptions for controlled substances or getting prescriptions from medical offices that engage in unethical practices

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



# Claims Get Processed Each Day_Outpatient
- Claim processing duration: 1.4 days in average
- Frequency of running model: Daily
- 1,415 claims are processed each day in average

![download (1)](https://github.com/LynnSynuo/Health_Insurance_Fraud_Detector/assets/117470609/71c4d7be-998e-41c0-a9e2-7ee53c2a1b89)


