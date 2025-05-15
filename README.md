# Hospital-Emergency-Dashboard (Interactive Dashboard creation using Ms Excel)
## Project Objective
I developed a comprehensive project in Excel, creating multiple dashboards and tables to analyze the data. This process involved several stages, including data preprocessing, data cleaning and data visualization.
## Dataset used
https://github.com/aman0816/Hospital-Emergency-Dashboard/blob/main/Dataset%20Hospital%20Emergency%20Room.csv

We need to create a Hospital Emergency Room Analysis Dashboard in Excel to improve efficiency and provide useful insights. This dashboard will help stakeholders monitor, analyze, and make better decisions for managing patients and improving services

KPI’S Requirement
Number of Patients: Count the total number of patients visiting the ER each day. Show a daily trend with an area sparkline to spot patterns like busy days or seasonal trends.
 Average Wait Time: Find the average time patients wait to see a medical professional. Use an area sparkline to track daily changes and highlight days with longer wait times that might need improvements.
 Patient Satisfaction Score: Check the average daily satisfaction score of patients to assess service quality. Use an area sparkline to show trends, spot drops in satisfaction, and link them to busy times or challenges.

Charts to Create: 
Patient Admission Status: Show how many patients were admitted vs. not admitted.
 Patient Age Distribution: Group patients by age.
 Timeliness: Measure the percentage of patients seen within 30 minutes.
 Gender Analysis: Display the number of patients by gender.
 Department Referrals: Check which departments patients are referred to the most.
 
Calendar Table Formula
 = List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))
 
DAX Formulas
DAX Formula for Age Group : 
=IF([Patient Age]>=70,"70-79",IF([Patient Age]>=60,"60-69",IF([Patient Age]>=45,"45-59",IF([Patient Age]>=30,"30-44",IF([Patient Age]>=15,"15-29",IF([Patient Age]>=5,"05-14","0-4")))))) 

DAX Formula For Patient Attend Status :
 =IF([Patient Waittime]<30,”Within Time”, “Delay”)

 Conclusion
 While the ER is handling a balanced number of admissions and has a manageable average wait time, the patient satisfaction score and delay rate indicate significant scope for process improvement. Targeted strategies in workflow optimization, staff training, and departmental coordination can enhance overall care delivery

## Dashboard Image 
https://github.com/aman0816/Hospital-Emergency-Dashboard/blob/main/Image_Hospital_Emergency_room_dashboard.PNG



