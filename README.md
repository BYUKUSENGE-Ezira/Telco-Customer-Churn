# Telco Customer Churn & Retention Analytics

A data preprocessing and exploratory data analysis (EDA) pipeline engineered with Python and Pandas to uncover behavioral patterns, demographic risk factors, and account configurations driving customer attrition for a telecommunications provider.

## 1. Project Overview
Customer attrition (or churn) presents a significant financial challenge for telecommunication firms. This project processes historical subscriber records to isolate the root indicators of service cancellation. By mapping out subscriber profiles—ranging from basic demographics to billing infrastructures—this analytics framework identifies high-risk cohorts and surfaces actionable insights to optimize targeted customer retention campaigns.

## 2. Strategic Objectives
* **Data Ingestion & Integrity:** Import structural data arrays, evaluate feature coverage, and diagnose data schema alignments.
* **Feature Engineering & Coercion:** Correct mismatched attribute classes, parse hidden missing values masked as whitespace data, and convert categorical classification metrics into binary parameters.
* **Missing Value Remediation:** Audit database column vectors for active null records and purge incomplete accounts to ensure unbiased data exploration.
* **Exploratory Risk Profiling:** Build descriptive visualizations linking customer segment choices directly with historical cancellation outcomes.

## 3. Tech Stack & Environment
* **Core Runtime:** Python 3.x
* **Data Engineering:** Pandas, NumPy
* **Data Visualization:** Seaborn, Matplotlib
* **Execution Environment:** Jupyter Notebook / Kaggle Kernels

## 4. Data Preprocessing Pipeline
The raw dataset underwent a rigorous data cleaning pipeline prior to exploration:
1. **Target Feature Encoding:** Converted the string target variable `Churn` (`Yes`/`No`) into a binary numeric scheme (`1`/`0`) to facilitate direct probability and average risk ratio calculations.
2. **Schema Alignment:** Discovered that `TotalCharges` was loaded as an un-calculable text `object` string type due to empty space strings. Coerced the column vector into a float numeric class, shifting hidden space placeholders into real tracking `NaN` properties.
3. **Null Purging:** Audited the data frame for missing rows and safely purged the newly unmasked null counts, ensuring structural consistency across all downstream analytics layers.

## 5. Exploratory Data Analysis Structure
Subscriber churn metrics were benchmarked across three core diagnostic divisions:
* **Demographic Vectors:** Evaluating customer segment distributions across Gender profiles, Senior Citizen status, Partner connectivity, and Dependents indicators.
* **Core Infrastructure:** Grouping churn rates against basic utility parameters, specifically inspecting Phone Service availability.
* **Account Configuration:** Mapping cancellation velocities against contract binding frameworks (Contract Type), digital invoicing setups (Paperless Billing), and transaction processing architectures (Payment Method).

## 6. Analytical Insights & Key Findings
* **Demographic Vulnerabilities:** Senior citizens exhibit an elevated attrition curve compared to younger groups. Similarly, independent subscribers without family connections (`Partner: No` or `Dependents: No`) present a substantially higher defection profile.
* **Contract Binding Influence:** Agreement structures hold the highest retention weight. Short-term Month-to-month subscribers represent an extreme churn risk profile, whereas 1-year and 2-year commitments anchor long-term consumer stability.
* **Accounting Infrastructure Risks:** Accounts settling fees via manual "Electronic check" actions show a massive churn spike. Conversely, automated workflows (Credit Card or direct Bank Transfers) reflect highly durable and loyal consumer relationships.
* **Agnostic Attributes:** Customer gender and base phone landline availability demonstrated nominal variance in attrition behavior, indicating they are neutral elements in retention evaluations.

## 7. Dataset Architecture
The raw records utilized in this development pipeline are sourced from the **Telco Customer Churn Database** available on Kaggle. It covers historical subscriber behavior metrics, active service enrollments, billing frequencies, and termination log results.

## 8. Conclusion & Core Takeaways
This analysis pinpoints definitive structural and behavioral drivers of account termination, with contract commitment type and payment selection representing the most critical levers for subscriber stability. Leveraging these insights allows management teams to transition from reactive loss management to proactive retention marketing. Note that these identified correlations represent behavioral associations rather than an absolute statement of direct psychological causation.
