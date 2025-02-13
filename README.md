
# Exploratory Data Analysis (EDA) on Medical Appointments Data (Python)

## Overview
This project performs an exploratory data analysis (EDA) on medical appointments to understand the factors that influence patient attendance. The dataset contains information about patients, their scheduled appointments, medical conditions, and whether they showed up for their appointments.

## Dataset Information
- **Total Records:** 110,527
- **Columns:** 14
- **Target Variable:** `NoShow` (Indicates whether a patient attended their appointment)

## Data Cleaning and Preprocessing
- Converted `ScheduledDay` and `AppointmentDay` to datetime format.
- Extracted weekday information for both scheduled and appointment days.
- Renamed columns for consistency (`Hipertension` → `Hypertension`, `Handcap` → `Handicap`, etc.).
- Dropped irrelevant columns (`PatientId`, `AppointmentID`, `Neighbourhood`).
- Categorized `Age` into groups.
- Checked for missing values and found none.
- Converted categorical variables into dummy variables for further analysis.

## Key Findings
### Gender Distribution
- Female patients have more appointments than male patients.

![image](https://github.com/user-attachments/assets/5e03734f-d6a7-4589-b645-b5e5ad85178a)


### No-show Rate
- **79.8%** of patients attended their appointments.
- **20.2%** of patients did not show up.

### Age Influence
- Attendance is similar across age groups, except for very young patients (Age 0-1), who have an **80% show-up rate**.

![image](https://github.com/user-attachments/assets/de3a9636-a81d-4a5d-b85e-d63505f94672)


### Neighborhood Attendance Rate
- Approximately **80%** of patients in each neighborhood showed up.

### Scholarship Impact
- Patients **without a scholarship** had an **80% show-up rate**.
- Patients **with a scholarship** had a **75% show-up rate**.

![image](https://github.com/user-attachments/assets/6b41bdbf-d756-4d35-8ed4-6091102c7b72)


### Medical Conditions and Attendance
- **Hypertension patients**: **85% attendance rate**.
- **Diabetic patients**: **83% attendance rate**.
- **Patients without these conditions**: **80% attendance rate**.

![image](https://github.com/user-attachments/assets/844852dd-4d63-4f52-bfd2-ae4088e3eaf7)

### SMS Reminders
- **Patients who did NOT receive an SMS reminder** had an **84% show-up rate**.
- **Patients who received an SMS reminder** had a **72% show-up rate**.

![image](https://github.com/user-attachments/assets/3286c987-2206-41ff-a9e0-a1c1bb2d9453)

### Weekday Analysis
- **No appointments on Sundays**.
- **Saturday has the lowest number of appointments compared to weekdays**.
![image](https://github.com/user-attachments/assets/6ac442e5-227a-48ad-9a96-0a46bc939dde)


## Conclusion
The analysis provides valuable insights into patient attendance behavior. Some interesting observations include the negative impact of SMS reminders on attendance and the higher attendance rates among patients with chronic conditions. These insights can help improve medical scheduling and patient engagement strategies.

---

## Next Steps
- Build predictive models to identify high-risk no-show patients.
- Analyze external factors like weather and transportation.
- Implement and test new patient reminder strategies.




