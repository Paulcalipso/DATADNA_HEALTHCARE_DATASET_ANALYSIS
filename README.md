# DATADNA HEALTHCARE DATASET ANALYSIS

# TABLE OF CONTENT
- DATADNA HEALTHCARE DATASET ANALYSIS - OVERVIEW
- OBJECTIVES OF THE ANALYSIS
- DATA SOURCE
- DESCRIPTION OF DATA
- DATA PREPROCESSING
- EXPLORATORY DATA ANALYSIS (EDA)
- DATA VISUALIZATION
- INSIGHTS
- RECOMMENDATIONS

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
An exploratory analysis was conducted on the dataset to identify key performance indicators (KPIs). The results are as follows:
- Total Patients Admitted: 55,500
- Total Billing Amount: $1.42 billion
- Average Length of Stay: 15.51 days
- Number of Hospitals: 10

New columns created using DAX formulas as follows: 
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

![Screenshot 2025-05-11 132538](https://github.com/user-attachments/assets/9fedc0c5-5cce-4f04-b9fb-91c353154e57)


# DATA VISUALIZATION

![DataDNA 1](https://github.com/user-attachments/assets/8445c34f-4d4c-4720-b958-f7595f255f23)
![DataDNA 2](https://github.com/user-attachments/assets/5e425e51-6dc1-4886-8016-0753ed7bf2d6)
![DataDNA 3](https://github.com/user-attachments/assets/248186dd-3757-480b-b978-4528301a4e74)

# INSIGHTS
Key insights derived from the exploratory data analysis are as follows:
- Gender Distribution:
The majority of admitted patients were female with approximately 27.75K (50%) admissions, followed by male patients at 22.20K (40%), and non-binary patients at 5.55K (10%).
- Top Blood Types by Admission:
  The three most commonly admitted blood types were:
  * A+ with 19.4K admissions
  * O+ with 13.9K admissions
  * O- with 8.3K admissions
- Age Group Distribution:
The 60+ age group recorded the highest number of admissions (21,148), while the 0–17 age group had the lowest (116 admissions).
- Top Diagnosed Medical Conditions:
  The three most diagnosed conditions were:
  * Diabetes – prevalent among patients with blood types A-, B+, and O+
  * Hypertension – commonly seen in A+ and O+ blood types
  * Obesity – found among A-, AB-, AB+, B-, and O- blood types
- Most Prescribed Medications by Condition:
  * Diabetes: Ibuprofen, Lipitor
  * Hypertension: Aspirin, Penicillin
  * Obesity: Paracetamol, Lipitor
  * Arthritis: Paracetamol, Lipitor
  * Cancer: Aspirin, Penicillin
  * Asthma: Paracetamol, Aspirin
- Admission Type and Billing:
Elective admissions accounted for the highest total billing amount.
- Insurance Providers by Gender:
  * Medicare primarily covered female patients, resulting in the highest billing contribution.
  * UnitedHealthcare and Aetna primarily covered male patients.
  * Cigna was the main provider for non-binary patients.
- Hospital Admissions:
  * Houston Methodist Hospital had the highest number of admissions with 20.40K.
  * NewYork-Presbyterian Hospital recorded the lowest at 2.33K.
- Regional Billing Totals:
  * The South region generated the highest billing amount at $520.98 million.
  * The Midwest region had the lowest billing at $125.23 million.

# RECOMMENDATIONS
- Targeted Healthcare Programs for Older Adults
  * With the 60+ age group representing the highest admissions, implement specialized geriatric care programs and chronic disease management initiatives tailored to this demographic.
  * Increase resource allocation (e.g., staffing, equipment) in departments serving older patients.
- Gender-Specific Health Outreach
  * Since females account for 50% of admissions, prioritize preventive care programs, wellness campaigns, and screenings targeting women's health.
  * Collaborate with Medicare to expand support for female patients, given their significant contribution to total billing.
- Enhance Elective Admission Efficiency
  * Given that elective admissions drive the highest billing, improve scheduling, pre-authorization, and patient education processes to reduce cancellations and delays.
  * Evaluate opportunities to increase elective procedure capacity where demand is high.
- Regional Resource Allocation
  * Allocate more funding, infrastructure, and staffing to the South, which has the highest billing volume, to support demand and sustain care quality.
  * Investigate and address potential inefficiencies or unmet needs in the Midwest, where billing is lowest.
- Hospital-Specific Planning
  * Support Houston Methodist Hospital with additional resources or expansion strategies due to its high patient load.
  * Analyze reasons behind low admissions at NewYork-Presbyterian Hospital to identify and address operational or outreach gaps.
- Insurance Partnership Optimization
  * Strengthen partnerships with top insurers (Medicare, UnitedHealthcare, Aetna, Cigna) to align service offerings with patient demographics and ensure comprehensive coverage.
  * Consider negotiating better rates or bundled service offerings with insurers covering high-volume patients.
