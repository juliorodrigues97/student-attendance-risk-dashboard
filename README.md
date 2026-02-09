# Attendance & Risk Monitoring Dashboard — Cultura Inglesa

## Project Overview
This project supports student retention through preventive and prescriptive analytics. It monitors attendance patterns, identifies students at risk of dropout, and triggers coordinated actions between branch managers, teachers, and the central office team. The dashboard is designed to ensure timely intervention, standardized follow-up, and clear prioritization of at-risk students.

## Business Problem
Student absenteeism is one of the main early indicators of disengagement and potential enrollment cancellation. Prior to this project, the organization lacked a structured and standardized process to identify at-risk students, track weekly absences, and document follow-up actions across branches. This limited the ability of managers and the coordination team to act quickly and consistently.

## Solution Approach
The solution was designed as an operational workflow supported by analytics, combining weekly monitoring and short-term risk assessment.

The Power BI dashboard is structured into three complementary pages:

### Page 1 — Operations Overview
•	Target audience: Central Office (analysts, coordinators, general manager)
•	Purpose: Monitor student risk over the last 30 days
•	Analysis by branch, level, and shift
•	Used weekly for macro-level monitoring and prioritization

### Page 2 — Weekly Operations
•	Target audience: Branch Managers
•	Purpose: Identify students with critical weekly absenteeism
•	Used every Friday as the main operational trigger
•	Displays only students who missed all classes in the week (2/2)
•	Includes an action button to register follow-up via an Excel form

### Page 3 — Students at Risk
•	Target audience: Analysts and Coordination Team
•	Purpose: Monitor students classified by 30-day risk level
•	Tracks intervention type, status, and history
•	Includes an action button to register interventions via an Excel form
•	Supports prioritization of students with higher risk or no prior intervention

## Business Rules
### Weekly Attendance Rules
•	Priority: Student missed 100% of weekly classes (2 out of 2)
•	Attention: Student missed 1 class in the week
•	Normal: Student had full attendance (0 absences)
•	The Weekly Operations page displays only Priority students

### 30-Day Risk Classification Rules
•	High Risk: 5 or more absences in the last 30 days
•	Medium Risk: 3 or more absences in the last 30 days
•	Normal: less than 3 absences in the last 30 days

## Key Decisions Enabled
•	Identify students requiring immediate follow-up
•	Prioritize coordination efforts based on risk severity
•	Ensure no at-risk student remains without registered intervention
•	Standardize follow-up and intervention history across branches

## Data Source & Preparation
•	Data was simulated using Python, based on a real operational context from a previous internship experience.
•	The dataset was designed to reflect realistic attendance patterns, risk distribution, and intervention scenarios.
•	Data cleansing, transformation, and modeling were applied before loading into Power BI.

## Scope & Limitations
•	Focused on preventive and prescriptive analytics
•	Does not evaluate post-intervention effectiveness
•	Outcome analysis identified as a potential future phase

## Tools & Technologies
•	Power BI
•	DAX
•	Power Query
•	Python (data simulation and preprocessing)
•	Excel Forms (intervention and follow-up records)
