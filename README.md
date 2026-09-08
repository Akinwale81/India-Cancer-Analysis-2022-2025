# India Cancer Analysis (2022-2025)
Data analysis and power BI dashboard analysing cancer patients data from 2022-2025

## Project Overview
This project analyses cancer patient data in India from 2022 to 2025 using Microsoft Power BI. The dashboard provides insights into patients distribution, treatment patterns, trends, and survival outcomes.

## Objectives
The main objectives of this project are to:
- Analyse the total number of cancer patients.
- Examine gender and age distribution.
- Examine the patient distribution across states.
- Analyse patients by age category
- Identify treatment patterns and trends.
- Analyse survival outcomes.
- Develop an interactive Power BI dashboard.
- Generate data driven insights and recommendations.

- ## Dataset
The dataset contains cancer patient records covering the period from 2022 to 2025.
The key variables used in the analysis include:

- **Age** - Patient's age.
- **Age Category** - Grouped age ranges used for demographic analysis.
- **Gender** - Patient's gender.
- **State** - Indian states associated with the patient record.
- **Cancer Type** - Type of cancer diagnosed.
- **Stage** - Cancer stage at the time of the record.
- **Treatment Type** - Type of treatment received.
- **Status** - Patient outcome/status.
- **Survival Months** - Number of months associated with patient survival.
 
  - ## Tools Used
  The following tools were used
- Microsoft Power BI - Dashboard development and data visualisation.
- Power Query - Data cleaning and transformation.
- DAX - Analytical calculations and measures.

## Data Preparation
The dataset was prepared using Power Query before analysis. The data preparation process included:

- Reviewing the structure of the dataset.
- Checking and correcting the data type.
- Identify missing values.
- Checking for duplicate records.
- Reviewing inconsistent values.
- Standardising relevant categorical fields.
- Transforming data fields.
- Creating a diagnosis year field.
- Preparing age category field.

 ## Exploratory Data Analysis (EDA)
After preparing the dataset Exploratory Data Analysis was performed to understand the characteristics and patterns within the data before developing the final dashboard. The EDA focused on the following:

### Patient Demographics
The distribution of patients was explored by Gender, Age and Age Category.
This provided an initial understanding of the demographic composition of the dataset.

### Geographical Distribution
Patient records were examined by state to identify locations with higher patient representation.

### Cancer Distribution 
The dataset was explored according to Cancer Type and Cancer Stage.
This helped identify the distribution of patients across different cancer categories and stages.

### Treatment Analysis
Treatment types were explored to understand how patients were distributed across the available treatment categories.

### Diagnosis Trends
Patients records were examined by diagnosis year to identify changes between 2022 and 2025

### Patient Status
Patient records were taken according to recorded status, including alive and deceased categories

### Survival Exploration 
Survival months were examined across different dimensions including:
- Treatment Type
- Cancer Type
- Age Category
- Cancer Stage
- Patient Status
The EDA stage helped determine which variables and relationships were most relevant for inclusion in the Power BI dashboard.

## Data Modelling and DAX
The model allows the dashboard to analyse patient information across different dimensions, including:
- Diagnosis Year
- State
- Cancer Type
- Cancer Stage
- Treatment Type
- Age Category
- Patient Status

### DAX Measures
DAX was used to create dynamic measures for the dashboard. Key measures include:
- Total Patients
- Male Patients
- Female Patients
- Male Percentage(%)
- Female Percentage(%)
- Average Age
- Average Survival Months
- Maximum Survival Months
 
This measures were used to populate KPI cards and analytical visualisations throughout the dashboard.

## Dashboard Development
The final Power BI dashboard was organised into three analytical pages. The pages use KPI cards to present key demographic measures.
  
### Overview
This provides a high level summary of the patient population. It includes:
- Total Patient
- Male Patients
- Male Percentage
- Female Patient
- Female Percentage
- Average Age
- Top 5 States
- Cancer Types
- Age Categories
- Cancer Stages.

[Overview](....)

### Treatment and Trends
This page focuses on treatment patterns and changes over time. It includes:
- Patients by Cancer Type
- Patients by Diagnosis Year
- Patients by Status
- Patients by Treatment Type

[Treatment and Trends](....)

### Survival Analysis
This page focuses on patient survival outcomes. It includes:
- Average Survival Months
- Average Survival Months for Alive Patients
- Average Survival Months for Deceased Patients
- Maximum Survival Months
- Survival by Treatment Type
- Survival by Cancer Type
- Survival by Age Category
- Survival by Cancer Stage

[Survival Analysis](....)

## Key Insights
- Patient Demographics: The gender and the age analysis provides an overview of the demographic composition of the patient population. The report shows 99,938 total patients. The female gender has the highest number of patients with 67,108, which is valued at 67.15% of the total patients while the male gender with the total number of 32,830, which is valued at 32.85% 0f the total patients. The report also has the record of 54 as the average age of the recorded patients.

- Geographical Distribution: The top 5 states analysis identifies states with the highest representation within the dataset. The report highlighted Delhi with the highest number of patients with a total number of 19,926 patients. Karnataka, Chandigarh, Gujarat and Kerala complete the top 5 states with the highest number of patients.

- Diagnosis Trend: The yearly analysis allows patient representation to be compared across 2022 to 2025. The report shows slight difference among the years in view. Year 2024 has the highest number of 25,100 patients, 2022 recorded a total number of 25,063 patients, year 2023 had a number of 24,918 patients and year 2025 has the least number of patients with 24,857.

- Cancer Type: The cancer type highlights the distribution of patients across different cancer categories. Breast cancer recorded the highest number of patients with a total number of 28,149, representing 28.17%. Ovarian cancer has the least number of patients with 3,903, representing 3.91%. The other cancer recorded are Oral cancer, Cervical cancer, Lung cancer, Colorectal cancer, Stomach cancer, Prostate cancer, Leukemia cancer.

- Cancer Stage: The stage analysis provides an overview of patient distribution across different stages of cancer. The analysis shows Stage III as the stage with the highest number of patients with 35,240, representing 35.26%, Stage II has 24.91% of the distribution, Stage IV with a distribution of 24.77% and the lest on the distribution is Stage I, with a number of 15,046 patients, representing 15.06%.

- Treatment Patterns: The analysis shows how patients are distributed across the recorded treatment categories. The pattern shows a total number 21,093 patients under the Palliative care treatment type, with surgery as the second highest treatment type with 20,618 patients. Others are Chemotheraphy, Targeted Therapy, Radiation, Chemo + Radiation and Surgery + Chemotheraphy, as the least patients distribution.

- Survival Outcome: The analysis enables comparison of average survival months across treatment type, cancer type, age categories and cancer stage.

## Recommendations
Based on the analysis, the following recommendations are proposed:

- Strengthen Regional Healthcare Planning: The dashboard identifies the states with the highest representation of cancer patients. States with the highest number of cases may require closer examination of healthcare capacity, including availability of oncology facilities, diagnostic services, specialist healthcare professionals, treatment centers and patient support services.

- Improve Early Detection and Stage Based Analysis: Cancer stage is an important variable in the dataset because it provides an indication of disease progression at diagnosis. Healthcare organisations could strengthen early detection initiative through increased public awareness campaigns, improved access to screening services, earlier diagnostic testing, community based screening programmes, faster communication of diagnostic results.

- Expand the Time-Series Analysis: Although this provides useful information about changes over the four year period, a four year period may not be sufficient to establish long term trends. The dataset should be updated regularly as new records become available.

- Establish Regular Performance Reporting: Rather than treating the dashboard as a one time analysis, it could be developed into a recurring reporting system. Regular reporting would allow stakeholders to monitor whether observed patterns are changing overtime. A monthly, quarterly or annual reporting cycle could be established depending on data availability.
- 
  

      - 
