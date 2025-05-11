# DATADNA HEALTHCARE DATASET ANALYSIS

# TABLE OF CONTENT
- DATADNA HEALTHCARE DATASET ANALYSIS - OVERVIEW
- OBJECTIVES OF THE ANALYSIS
- DATA SOURCE
- DESCRIPTION OF DATA
- DATA PREPROCESSING
- EXPLORATORY DATA ANALYSIS (EDA)
- 

# DATADNA HEALTHCARE DATASET ANALYSIS - OVERVIEW
This project involves the development of an interactive Power BI dashboard to analyze and visualize patient care data from 55,500 unique records across 10 major hospitals in the United States. The dataset includes detailed information on hospital admissions, medical conditions, prescribed medications, insurance providers, and treatment costs.
The goal is to uncover actionable insights that can drive better healthcare decisions, reduce costs, and improve patient outcomes. By identifying trends and performance indicators across hospitals, the dashboard will serve as a strategic tool for healthcare administrators and stakeholders to make informed, data-driven decisions and enhance the overall quality of care

# OBJECTIVES OF THE ANALYSIS
Key questions to answer in this analysis are:
- What are the most common age groups, genders, and blood types among patients, and are certain groups being admitted more frequently than others?
- Which medical conditions are diagnosed most often, and do these conditions disproportionately affect specific demographic groups?
- How long do patients typically stay in the hospital for various conditions, and does the length of stay differ by hospital or type of admission (emergency, urgent, or planned)?
- What are the average treatment costs for different conditions, and are there significant cost variations between hospitals or insurance providers?
- Which hospitals are treating the highest number of patients, and how do they compare in terms of patient outcomes, such as test results?
- What medications are most commonly prescribed for each condition, and are these medications used consistently across different hospitals?
- How are patients most commonly admitted—through emergency, urgent, or planned admissions—and how does the admission type affect length of stay and treatment costs?
- Which insurance providers cover the largest number of patients, and how does insurance coverage relate to treatment costs and patient outcomes?
- Where are the hospitals located, and are there any regional differences in health conditions, quality of care, or billing amounts?

# DATA SOURCE
This dataset is gotten from Onyxdata.co.uk [LINK TO PORTFOLIO](https://datadna.onyxdata.co.uk/portfolio/)

# DESCIPTION OF DATA
The dataset contains columns such as:
- Patient ID – Unique identifier for each patient
- Age – Patient’s age
- Gender – Gender of the patient
- Blood Type – Patient’s blood group
- Medical Condition – Diagnosed health issue(s)
- Date of Admission – When the patient was admitted
- Doctor – Attending physician
- Hospital – Name of the hospital providing care
- Insurance Provider – Company covering the patient’s treatment
- Billing Amount – Total cost of treatment
- Room Number – Assigned hospital room
- Admission Type – Nature of the admission (e.g., emergency, urgent, planned)
- Discharge Date – When the patient was released from the hospital
- Medication – Drugs prescribed during the stay
- Test Result – Outcome of medical tests
- Hospital Latitude – Geographic location of the hospital

# DATA PREPROCESSING
- Data Transformation - The followng task were carried out:
  * Ensured the dataset contained no duplicate values to maintain data integrity and prevent skewed results.
  * Verified that there were no missing values or blank cells to ensure completeness and accuracy of the analysis.
  * Checked and standardized column formats (e.g., dates, numerical values, categorical data) to enable consistent and reliable reporting in Power BI.

# EXPLORATORY DATA ANALYSIS (EDA)
new columns were created - 
- Age Groups: Categorized patient ages into four defined groups for easier demographic analysis:
  * 0-17
  * 18-39
  * 40-59
  * 60+
- Length of stay: Calculated by finding the difference in days between the Date of Admission and the Discharge Date, to measure how long patients stayed in the hospital.
- USRegion: Created to classify hospitals by geographic region for regional analysis:
  * West - hospitals in this regions are:
    - Cedars-Sinai Medical Center
    - UCLA Medical Center
    - UCSF Medical Center
  * Midwest - hospitals in this region are:
    - Mayo Clinic
    - Northwestern Memorial Hospital
  * South - hospital in this region is:
    - Houston Methodist Hospital
  * Northeast - hospitals in this region are:
    - Cleveland Clinic
    - Johns Hopkins Hospital
    - Massachusetts General Hospital
    - NewYork-Presbyterian Hospital
- Admission Year: Extracted the year from the Date of Admission column to analyze trends over time (2019–2024).
