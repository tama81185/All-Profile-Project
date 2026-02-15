# Construction Performance Analysis Dashboard

##  Project Overview

This project analyzes construction project performance across multiple regions, departments, contractors and project phases.  

The objective is to provide centralized visibility into financial performance, safety incidents, contractor efficiency and monthly operational trends through an interactive dashboard.

Without a centralized reporting system:
- Budget overruns are difficult to detect early.
- Contractor performance is not consistently monitored.
- Safety risks are not clearly analyzed by region or phase.
- Monthly performance trends are not systematically tracked.
- Decision-making relies heavily on manual reports and spreadsheets.

This dashboard solves these challenges by providing a data-driven, visual reporting solution.

---

#  Live Dashboard  
👉 **[Click here to view the interactive dashboard](https://lookerstudio.google.com/reporting/ab05cb99-e2a3-4c27-815e-491b5ad5160c/page/EmVoF)**

---

# Dashboard Pages

---

#  Overview Page: High-Level Project Metrics

The **Overview Page** provides a snapshot of the key metrics for all tracked projects.

##  KPI Cards

- **# of Projects** – Displays the total number of projects being tracked.
- **Total Budget** – Sum of allocated budgets across all projects.
- **Total Cost** – Sum of actual project costs.
- **Cost per Project** – Average cost across projects.
- **Safety Incidents** – Total number of reported workplace accidents across all projects.

##  Charts

- **# of Projects by Region** – Shows the number of projects by geographic region (North, South, East, West).
- **# of Projects by Status** – Breaks down projects by their current status (Completed, In Progress, Pending).
- **# of Projects by Phase** – Categorizes projects by Design, Construction, and Finishing phases.
- **# of Projects by Month Name** – Tracks project activity month-over-month.
- **Cost per Project by Project Type** – Displays cost comparison across Industrial, Residential, and Commercial projects.

Construction_Performance/images/overview.png

This page provides a comprehensive overview of the construction portfolio, enabling executives to monitor financial health, workload distribution, and safety performance at a glance.

---

# 2️⃣ Budget vs Cost Page: Comparing Project Budgets with Actual Costs

The **Budget vs Cost Page** allows management to compare allocated budgets against actual spending and detect cost overruns.

## 📈 Charts

- **Budget and Cost by Department** – Displays financial performance across Engineering, Safety, and Procurement.
- **Budget and Cost by Project Type** – Compares financial performance across Industrial, Residential, and Commercial projects.
- **Budget and Cost by Region** – Identifies regional financial discrepancies.
- **Budget and Cost by Top 7 Contractors** – Evaluates contractor-level cost performance.

📸 *(Insert Budget vs Cost Screenshot Here)*

This page is essential for identifying overspending departments, high-cost regions, and contractors that consistently exceed budget expectations.

---

# 3️⃣ Contractor & Department Performance Page

This page focuses on operational workload and contractor accountability.

## 📈 Charts

- **Projects by Contractor** – Identifies contractors managing the most projects.
- **Safety Incidents by Contractor** – Highlights contractors with recurring safety issues.
- **Projects by Department** – Shows workload distribution across departments.
- **Budget Variance by Contractor** – Displays cost performance at contractor level.

📸 *(Insert Contractor Performance Screenshot Here)*

This analysis supports better contractor evaluation, risk mitigation, and performance-based decision-making.

---

# 4️⃣ Safety & Risk Analysis Page

The **Safety & Risk Analysis Page** provides insights into workplace safety trends and high-risk areas.

## 📈 Charts

- **Safety Incidents by Region** – Identifies high-risk geographic areas.
- **Safety Incidents by Phase** – Analyzes risk exposure during Design, Construction, and Finishing.
- **Safety Incidents by Project Type** – Determines which project categories face higher safety risks.
- **Monthly Safety Trend** – Tracks safety incident patterns over time.

📸 *(Insert Safety Analysis Screenshot Here)*

This page enables proactive risk management and improved safety planning.

---

# 📂 Dataset Information

**Dataset:** `construction.csv`

### Key Fields:
- Project ID
- Region
- Department
- Contractor
- Project Type
- Project Phase
- Status
- Budget
- Actual Cost
- Safety Incidents
- Month Name

---

# 🎯 Key Performance Indicators (KPIs)

1. **Total Number of Projects** – Count of all projects in the dataset.
2. **Total Budget** – Sum of allocated budgets across all projects.
3. **Total Cost** – Sum of actual project costs.
4. **Cost per Project** – Average cost across projects.
5. **Safety Incidents** – Total number of reported workplace accidents.

---

# 💼 Business Impact

This dashboard enables:

- Early detection of budget overruns  
- Improved contractor performance monitoring  
- Enhanced safety risk analysis  
- Better resource allocation  
- Data-driven executive decision-making  
- Reduced reliance on manual reporting  

---

# 🛠 Tools Used

- Looker Studio (Dashboard Development)
- Excel / CSV Dataset
- GitHub (Version Control & Documentation)

---

# 🚀 Conclusion

The Construction Performance Analysis Dashboard centralizes financial, operational, and safety data into one interactive reporting system.  

It enhances transparency, improves accountability, and supports strategic decision-making across the organization.
