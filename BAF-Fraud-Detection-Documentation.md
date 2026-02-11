# BAF-Fraud-Detection-Documentation

[Download the Document (PDF)](https://github.com/mrlizhaozhi/application-fraud-bank-account-opening/blob/main/BAF-Fraud-Detection-Documentation.docx)

## Overview

Model Risk Management (MRM) is a critical aspect of any financial institution, especially those dealing with fraud detection. The Banking Anti-Fraud (BAF) Fraud Detection project aims to develop and implement an advanced machine learning model that can accurately identify fraudulent transactions in real time. This documentation aims to meet SR 11-7 standards.

## Supervisory Letter SR 11-7

SR 11-7 is a set of standards and guidelines developed by the Securities and Exchange Commission (SEC) to ensure that financial institutions have robust systems in place for detecting, preventing, and responding to fraud. The BAF Fraud Detection project aims to comply with these standards by developing an advanced machine learning model that can be deployed in production. Essential components of SR 11-7 include:

- **Definition of a Model**: Any quantitative method, system, or approach using statistical or economic theories to process data into estimates.

- **Model Validation**: An independent, comprehensive review to ensure models are accurate and appropriate for their intended use.

- **Governance and Controls**: Banks must establish strong policies, procedures, and accountability mechanisms for model development, implementation, and ongoing monitoring.

- **Scope**: Applies to all institutions supervised by the Federal Reserve or OCC, including national and state banks. 

## This documentation is consisted of the following componenets:

1. Model Identification and Purpose

    - **Model Name and Version**: Unique identifiers that track the specific iteration of the fraud model being deployed.

    - **Business Use Case**: A clear statement defining how the model detects specific fraud typologies within the BAF dataset, such as account takeover or synthetic identity fraud.

    - **Model Owner and Stakeholders**: Documentation of the individuals or teams accountable for the model’s performance and regulatory compliance.

2. Data Integrity and Lineage

    - **Data Sources and Scope**: A description of the input variables from the BAF dataset, including transaction attributes and behavioral features.

    - **Data Quality Assessment**: Evidence of checks for missing values, outliers, and data freshness to ensure the model isn't learning from "garbage" data.

    - **Feature Engineering Rationale**: An explanation of why specific derived features were created to capture complex fraud patterns.

3. Model Development and Methodology

    - **Algorithm Selection**: Justification for choosing specific architectures (e.g., Random Forest vs. Neural Networks) based on the BAF dataset's characteristics.

    - **Model Assumptions and Limitations**: A transparent list of what the model cannot do and the conditions under which it might fail.

    - **Training and Testing Split**: Details on how the data was partitioned to prevent data leakage and ensure the model generalizes well to unseen fraud.

4. Validation and Testing

    - **Performance Metrics**: Results of testing using metrics like Precision, Recall, and the Area Under the Precision-Recall Curve (AUPRC), which are critical for imbalanced fraud data.

    - **Sensitivity Analysis**: Documentation of how the model reacts to changes in input variables or shifts in fraudster behavior.

    - **Backtesting Results**: A comparison of predicted fraud vs. actual historical outcomes within the BAF suite to prove accuracy.

5. Implementation and Monitoring

    - **Deployment Environment**: A description of the technical infrastructure where the model resides and how it integrates with real-time payment rails.

    - **Ongoing Monitoring Plan**: The schedule and thresholds for tracking "model drift" to ensure the model stays effective as fraud tactics evolve.

    - **Change Management Process**: A formal protocol for how the model will be updated, retrained, or decommissioned in the future.