^^^^Purpose of this project^^^^
I created a Hospital Emergency Room Analysis Dashboard in Power BI to improve efficiency and provide useful insights. This dashboard will help stakeholders monitor, analyze, and make better decisions for managing patients and improving services.


^^^^Key Performance Indicator (KPI) Specifications^^^^

Core operational and patient-experience metrics designed to monitor daily Emergency Room (ER) volume, service efficiency, and care quality.

1. Daily Patient Volume (Number of Patients)

Definition & Calculation: Total count of unique patient visits to the Emergency Room per day.

Visualization: Primary KPI card paired with an area sparkline displaying daily visit trends.

Analytical Objective: Identify peak demand days, recurring weekly patterns, and seasonal volume surges to support staffing and capacity planning.

2. Average Patient Wait Time

Definition & Calculation: Mean duration (in minutes) elapsed between patient arrival/registration and initial consultation with a medical professional.

Visualization: Primary KPI card paired with an area sparkline tracking daily fluctuations.

Analytical Objective: Monitor service delivery efficiency, detect bottlenecks on high-latency days, and pinpoint operational opportunities to reduce patient wait times.

3. Average Patient Satisfaction Score

Definition & Calculation: Daily mean satisfaction rating recorded from post-visit patient feedback.

Visualization: Primary KPI card paired with an area sparkline illustrating daily sentiment trends.

Analytical Objective: Evaluate perceived quality of care, detect sudden declines in satisfaction, and correlate service drops with operational pressures such as peak volume or extended wait times.


^^^^Project Implementation Steps^^^^

Phase 1: Discovery & Data Ingestion

# Business Requirement Gathering

# Partner with stakeholders to define core business objectives, analytical questions, success metrics, and target KPIs.

# Data Exploration & Profiling

# Conduct initial data profiling to evaluate dataset granularity, schema structure, data types, and source-system limitations.

# Data Extraction & Ingestion (Power Query)

# Establish automated connections to raw data sources and ingest records into the analytical environment via Power Query.

Phase 2: Data Preparation & Modeling

# Data Cleansing & Quality Assurance (Power Query)

# Execute transformation pipelines to standardize data formats, resolve missing or inconsistent values, eliminate duplicates, and enforce data integrity.

# Date Dimension Engineering (Power Query)

# Construct a dedicated calendar dimension table to enable standardized time-series reporting and period-over-period comparisons.

# Relational Data Modeling (Power Pivot)

# Architect an optimized star-schema data model in Power Pivot by defining primary-to-foreign key relationships between fact and dimension tables.

# Analytical Calculations & KPIs (DAX)

# Author Data Analysis Expressions (DAX) to build custom calculated columns and dynamic measures that accurately reflect business logic.

Phase 3: Visualization & Decision Support

# Analytical Aggregation & Dashboard Wireframing

# Build core Pivot Table aggregations and design an intuitive, grid-aligned dashboard layout prioritized for executive readability.

# Data Visualization & Visual Formatting

# Develop tailored charts and apply consistent visual hierarchy, color encoding, and labeling to communicate patterns without clutter.

# Interactive Reporting & Dashboard Assembly

# Integrate dynamic slicers, cross-filtering, and KPI cards into a cohesive, self-service reporting interface.



^^^^Key Analytical Insights (Sample View: May 2023)^^^^

1. Patient Volume & Admission Outcomes

Monthly Throughput: The Emergency Room handled 480 total patient visits in May 2023.

Balanced Disposition Split: Nearly half of all ER arrivals required inpatient admission—229 patients (48%) were admitted, while 251 patients (52%) were treated and discharged without admission.

2. Wait Time & Service Timeliness Bottlenecks

Extended Average Wait Time: Patients waited an average of 34.4 minutes to be attended by a medical professional.

High Delay Rate: 74% of patients experienced delays beyond the target response threshold, with only 26% attended on time—indicating a clear operational bottleneck in triage or physician availability.

Moderate Patient Satisfaction: The average patient satisfaction score stood at 5.16 (out of 10), reflecting the operational strain caused by elevated wait times and delayed consultations.

3. Demographic Breakdown (Age & Gender)

Peak Age Cohort: The 30–39 age group accounted for the highest visit volume (73 patients), followed closely by pediatric patients aged 0–09 (63 patients) and adults aged 40–49 (63 patients).

Lowest Volume Cohort: Teenagers aged 10–19 represented the smallest segment (49 patients).

Gender Distribution: Female patients comprised a slight majority at 54%, compared to 46% male patients.

4. Departmental Referral Patterns

Primary ER Resolution: The vast majority of cases (604 across the active referral view) required no external department referral, demonstrating that most visits were managed directly within the Emergency Room.

Top Specialist Referrals: Among referred cases, General Practice (195) and Orthopedics (86) accounted for the highest specialist demand, followed by Physiotherapy (35), Neurology (27), Cardiology (23), Gastroenterology (20), and Renal (9).


^^^^Actionable Recommendations^^^^

Optimize Peak-Hour Staffing: Align physician and triage nurse schedules with high-volume arrival windows to reduce the 34.4-minute average wait time and improve the 26% on-time rate.

Fast-Track General Practice & Non-Referral Cases: Since most patients do not require specialty inpatient referrals (or route to General Practice), introducing a dedicated fast-track triage lane for low-acuity cases can decompress main ER capacity.

Monitor Satisfaction Drivers: Track daily correlation between wait-time spikes and satisfaction scores (5.16) to evaluate the impact of triage workflow improvements.




