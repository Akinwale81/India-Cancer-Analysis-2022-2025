# India Cancer Analysis (2022-2025)
Interactive Power BI dashboard analysing cancer patient data in India from 2022-2025

## Dashboard Preview
![India Cancer Analysis Dashboard](https://github.com/Akinwale81/India-Cancer-Analysis-2022-2025/tree/main/Screenshots)

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
- Checking and correcting data types.
- Identifying missing values.
- Checking for duplicate records.
- Reviewing inconsistent values.
- Standardising relevant categorical fields.
- Transforming data fields.
- Creating a diagnosis year field.
- Preparing age category field.

 ## Exploratory Data Analysis (EDA)
After preparing the dataset Exploratory Data Analysis was performed to understand the characteristics and patterns within the data before developing the final dashboard. The EDA focused on the following:

### Patient Demographics
The distribution of patients was explored by Gender, Age and Age Category. The gender with the most representation was the female accounting to a total number of 67,108 patients which represent 67.25% of the distribution. The maximum age of patients was 95, while the minimum age was 1. The age category had ages grouped, with age between 1 and 30 grouped as child or young, age between 31 and 60 was grouped as Adult, age between 61 and 95 was grouped as Senior. The Adult age group has the highest representation with 63.64%.
This provided an initial understanding of the demographic composition of the dataset.

### Geographical Distribution
Patient distribution varied considerably across states, with Delhi recording the highest representation at 19,926 patients.

### Cancer Distribution 
The dataset was explored according to Cancer Type and Cancer Stage. Breast cancer has the highest representation of 28,149 patients, representing 28.17% of the distribution. Stage III also has the highest representation of 35,240 patients.
This helped identify the distribution of patients across different cancer categories and stages.

### Treatment Analysis
Treatment types were explored to understand how patients were distributed across the available treatment categories. The report shows a record number of 21,093 patients were placed under the palliative treatment type which makes the treatment type with the highest number of patients.

### Diagnosis Trends
Patients records were examined by diagnosis year to identify changes between 2022 and 2025. Year 2024 has the highest number of patients with 25,100.

### Patient Status
Patient records were taken according to recorded status, including alive and deceased categories. The report shows 63.58% were deceased, making it the category with the highest representation.

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
- Total Patients = COUNTROWS('india_cancer_patients_2022_2025 Cleaned')
- Male Patients = COUNTROWS(FILTER('india_cancer_patients_2022_2025 Cleaned','india_cancer_patients_2022_2025 Cleaned'[Gender]="Male"))
- Female Patients = COUNTROWS(FILTER('india_cancer_patients_2022_2025 Cleaned','india_cancer_patients_2022_2025 Cleaned'[Gender]="Female"))
- Male Percentage(%) = CALCULATE(DIVIDE('Measures (2)'[Male],COUNTROWS('india_cancer_patients_2022_2025 Cleaned')))
- Female Percentage(%) = CALCULATE(DIVIDE('Measures (2)'[Female],COUNTROWS('india_cancer_patients_2022_2025 Cleaned')))
- Average Age = AVERAGE('india_cancer_patients_2022_2025 Cleaned'[Age])
- Average Survival Months = AVERAGE('india_cancer_patients_2022_2025 Cleaned'[Survival_Months])
- Maximum Survival Months = MAX('india_cancer_patients_2022_2025 Cleaned'[Survival_Months])
 
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

[Overview](https://github.com/Akinwale81/India-Cancer-Analysis-2022-2025/blob/main/Screenshots/Overview.png)

### Treatment and Trends
This page focuses on treatment patterns and changes over time. It includes:
- Patients by Cancer Type
- Patients by Diagnosis Year
- Patients by Status
- Patients by Treatment Type

[Treatment and Trends](https://github.com/Akinwale81/India-Cancer-Analysis-2022-2025/blob/main/Screenshots/Treatment%20and%20Trend.png)

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

[Survival Analysis](https://github.com/Akinwale81/India-Cancer-Analysis-2022-2025/blob/main/Screenshots/Survival%20Analysis.png)

## Key Insights
- Patient Demographics: The gender and the age analysis provides an overview of the demographic composition of the patient population. The report shows 99,938 total patients. The female gender has the highest number of patients with 67,108, which is valued at 67.15% of the total patients while the male gender with the total number of 32,830, which is valued at 32.85% of the total patients. The report also has the record of 54 as the average age of the recorded patients.

- Geographical Distribution: The top 5 states analysis identifies states with the highest representation within the dataset. The report highlighted Delhi with the highest number of patients with a total number of 19,926 patients. Karnataka, Chandigarh, Gujarat and Kerala complete the top 5 states with the highest number of patients.

- Diagnosis Trend: The yearly analysis allows patient representation to be compared across 2022 to 2025. The report shows slight difference among the years in view. Year 2024 has the highest number of 25,100 patients, 2022 recorded a total number of 25,063 patients, year 2023 had a number of 24,918 patients and year 2025 has the least number of patients with 24,857.

- Cancer Type: The cancer type highlights the distribution of patients across different cancer categories. Breast cancer recorded the highest number of patients with a total number of 28,149, representing 28.17%. Ovarian cancer has the least number of patients with 3,903, representing 3.91%. The other cancer recorded are Oral cancer, Cervical cancer, Lung cancer, Colorectal cancer, Stomach cancer, Prostate cancer, Leukemia cancer.

- Cancer Stage: The stage analysis provides an overview of patient distribution across different stages of cancer. The analysis shows Stage III as the stage with the highest number of patients with 35,240, representing 35.26%, Stage II has 24.91% of the distribution, Stage IV with a distribution of 24.77% and the lowest proportion is Stage I, with a number of 15,046 patients, representing 15.06%.

- Treatment Patterns: The analysis shows how patients are distributed across the recorded treatment categories. The pattern shows a total number 21,093 patients under the Palliative care treatment type, making it the most frequently recorded treatment type, followed by surgery with 20,618 patients. Others are Chemotherapy, Targeted Therapy, Radiation, Chemo + Radiation and Surgery + Chemotherapy, as the least patients distribution.

- Survival Outcome: The analysis enables comparison of average survival months across treatment type, cancer type, age categories and cancer stage. According to the report, Surgery treatment type showed the highest survival rate at approximately 22.7 months on average. The report showed Prostate cancer type with the most average survival months rate at approximately 22.6 months. The report also showed Child or Young as the category by age with the most average survival months at approximately 20.8 months. Average survival months decreases as cancer stage increased, indicating poor survival outcome among patients recorded at more advanced stages. Stage I recorded approximately 24.1 months and the average survival months decreased as the cancer grew in stages.

## Recommendations
Based on the analysis, the following recommendations are proposed:

- Strengthen Regional Healthcare Planning: The dashboard identifies the states with the highest representation of cancer patients. States with the highest number of cases may require closer examination of healthcare capacity, including availability of oncology facilities, diagnostic services, specialist healthcare professionals, treatment centers and patient support services. The findings should be used to support evidence-based allocation of healthcare resources. However, patient counts should not be interpreted directly as population-level cancer incidence.

- Improve Early Detection and Stage Based Analysis: Stage III represented the largest proportion of recorded cancer cases. The relatively high representation of stage III cases highlights the importance of strengthening early cancer detection and screening programmes. Cancer stage is an important variable in the dataset because it provides an indication of disease progression at diagnosis. Healthcare organisations could strengthen early detection initiative through increased public awareness campaigns, improved access to screening services, earlier diagnostic testing, community based screening programmes, faster communication of diagnostic results.

- Expand the Time-Series Analysis: Although this provides useful information about changes over the four year period, a four year period may not be sufficient to establish long term trends. The dataset should be updated regularly as new records become available.

- Regular Monitoring: Healthcare organisations should regularly update and monitor cancer patient data to identify changes in patient demographics, cancer types, treatment patterns, cancer stages and survival outcomes.

- Establish Regular Performance Reporting: Rather than treating the dashboard as a one time analysis, it could be developed into a recurring reporting system. Regular reporting would allow stakeholders to monitor whether observed patterns are changing over time. A monthly, quarterly or annual reporting cycle could be established depending on data availability.

## Limitations
The analysis has some limitation, they are:
- The findings depend on the quality and completeness of the available dataset.
- The analysis is primarily descriptive and does not establish causal relationships.
- Patient representation in the dataset should not necessarily be interpreted as population-level cancer incidence.
- A longer time period would be useful for assessing long-term trends.
  

  
