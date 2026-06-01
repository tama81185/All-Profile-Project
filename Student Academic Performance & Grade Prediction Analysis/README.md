


## Project Title
**Student Academic Performance & Grade Prediction Analysis**

---

## Business Problem

Educational institutions often struggle to understand why students perform differently despite being in the same academic environment. School management lacks clear visibility into how study habits, absenteeism, parental involvement, tutoring and extracurricular activities influence student academic outcomes.

Without this understanding, schools face difficulties in:

- Identifying at-risk students early
- Designing effective intervention programs
- Optimizing attendance, tutoring and parental engagement policies
- Improving overall academic success rates

This limits data-driven academic planning and student support strategies.

---

## Business Objective

The goal of this project is to analyze historical student performance data to:

- Identify key factors influencing student GPA and grade classification
- Detect patterns leading to academic success or failure
- Classify students into grade categories (A–F)
- Predict student grade class using Machine Learning
- Provide actionable insights for early intervention and policy improvement
- Support educators and administrators in data-driven academic decision-making

---

## Data Source

**Dataset:** Student_performance_data_.csv

---

## Data Description

### Student Information

- **StudentID** → Unique identifier assigned to each student (1001–3392)

### Demographic Details

- **Age** → Student age (15–18)
- **Gender** → Gender of student
  - 0 = Male
  - 1 = Female

- **Ethnicity** → Student ethnicity
  - 0 = Caucasian
  - 1 = African American
  - 2 = Asian
  - 3 = Other

- **ParentalEducation** → Highest parental education level
  - 0 = None
  - 1 = High School
  - 2 = Some College
  - 3 = Bachelor's
  - 4 = Higher

### Study Habits

- **StudyTimeWeekly** → Weekly study hours (0–20)
- **Absences** → Number of absences in a school year (0–30)
- **Tutoring** → Tutoring participation
  - 0 = No
  - 1 = Yes

### Parental Involvement

- **ParentalSupport** → Level of parental support
  - 0 = None
  - 1 = Low
  - 2 = Moderate
  - 3 = High
  - 4 = Very High

### Extracurricular Activities

- **Extracurricular** → Participation in extracurricular activities
  - 0 = No
  - 1 = Yes

- **Sports** → Participation in sports
  - 0 = No
  - 1 = Yes

- **Music** → Participation in music
  - 0 = No
  - 1 = Yes

- **Volunteering** → Participation in volunteering
  - 0 = No
  - 1 = Yes

### Academic Performance

- **GPA** → Grade Point Average (2.0 – 4.0)

---

## Target Variable

### GradeClass

Grade classification based on GPA:

- **0 = A** (GPA ≥ 3.5)
- **1 = B** (3.0 ≤ GPA < 3.5)
- **2 = C** (2.5 ≤ GPA < 3.0)
- **3 = D** (2.0 ≤ GPA < 2.5)
- **4 = F** (GPA < 2.0)

---

## Key Performance Indicators (KPIs)

- **Average GPA** = Mean of GPA
- **Total Students** = Count of StudentID
- **Grade Distribution (%)** = Percentage of students in each GradeClass
- **At-Risk Student Rate** = Percentage of students in Grade D & Grade F
- **Average Study Time (hrs/week)**
- **Average Absences per Student**
- **Tutoring Participation Rate (%)**
- **Extracurricular Participation Rate (%)**

---

## Business Questions

### Academic Performance Analysis

- What factors most strongly influence student GPA and grade class?
- How does weekly study time impact academic performance?
- What is the relationship between absences and failure rates?
- Does parental support significantly improve student outcomes?
- How does parental education level affect student grades?
- Do students receiving tutoring perform better academically?
- Can extracurricular activities offset low study time?

### Risk Analysis

- Which combination of factors leads to the highest risk of academic failure?
- What percentage of academic failures are preventable through intervention?
- Which students should be flagged for early academic intervention?
- At which GPA level is intervention most effective?

### Demographic Analysis

- Are there performance differences across gender and ethnicity?

### Machine Learning & Prediction

- How accurately can student grades be predicted using Machine Learning?
- Which features are the most important predictors of academic performance?

### Strategic Decision-Making

- What academic policies provide the highest return on investment (ROI)?

---

## Expected Deliverables

- Exploratory Data Analysis (EDA)
- Student Performance Dashboard
- Academic Risk Assessment Report
- Grade Classification Analysis
- Machine Learning Prediction Model
- Feature Importance Analysis
- Actionable Recommendations
- Student Intervention Strategy

---

## Expected Business Impact

- Improve overall student academic performance
- Reduce failure rates
- Identify at-risk students earlier
- Increase effectiveness of tutoring programs
- Improve attendance management
- Enhance parental engagement
- Support data-driven academic planning
- Optimize educational resource allocation
