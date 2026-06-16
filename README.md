# Customer_Support_Performance_Dashboard

# Project Overview
Customer_Support_Performance_Dashboard | Personal Project | Jan 2026
• Developed an end-to-end Power BI dashboard using simulated BPO operational data.
• Designed Star Schema data model and implemented DAX measures.
• Created SLA, AHT, Occupancy, Productivity, and CSAT KPIs.
• Improved reporting visibility through drill-through and interactive dashboards.

# Business Problem
The customer support leadership team required a centralized analytics solution to monitor workforce performance, operational efficiency, customer satisfaction, and service quality across multiple teams and brands.

Operational data was distributed across various sources including attendance records, call statistics, productivity tracking, quality evaluations, customer satisfaction surveys, and auxiliary activity logs. This made it difficult for managers to gain a unified view of agent performance and identify areas requiring improvement.

The objective of this project was to develop an interactive Power BI dashboard that consolidates operational data into a single reporting platform, enabling stakeholders to:

• Monitor agent productivity and case resolution performance.
• Track attendance and workforce utilization.
• Analyze customer satisfaction (CSAT) trends.
• Evaluate quality assessment scores.
• Measure call handling efficiency and occupancy.
• Identify performance gaps and coaching opportunities.
• Support data-driven operational decisions.

# Solution Architecture

Excel Files / Source Data
        ↓
Power Query
        ↓
Data Cleaning & Transformation
        ↓
Star Schema Data Model
        ↓
DAX Measures & KPIs
        ↓
Interactive Power BI Dashboard
        ↓
Business Insights & Performance Monitoring

# Tools Used
Excel Dataset, 
Power BI

# Data Model
A dimensional data model was designed using a Star Schema approach to support efficient reporting and KPI analysis across customer support operations.

Dimension Tables:
• Dim_Agent – Agent details including Agent Name and Agent Number.
• Dim_Brand – Business brand information.
• Dim_Date – Calendar dimension containing Date, Day, Month, Week, Quarter, and Year attributes.
• Dim_Team – Team hierarchy and team-level information.

Fact Tables:
• Fact_CallStats – Call handling metrics including login time, available time, occupancy, working rate, inbound/outbound calls, and average talk time.
• Fact_Attendance – Agent attendance and workforce management metrics.
• Fact_Prod – Productivity metrics including cases worked, cases solved, solved rate, response time, and ticket category analysis.
• Fact_CSAT – Customer Satisfaction (CSAT) survey scores and customer feedback metrics.
• Fact_CSAT_End – Contact lifecycle and resolution tracking data.
• Fact_Quality – Quality assessment and agent evaluation scores.
• Fact_Aux – Auxiliary activity tracking including AUX codes, duration, and unavailable time categories.

Relationships:
All fact tables are connected to shared dimensions (Agent, Brand, Date, and Team) through one-to-many relationships, enabling cross-functional analysis across attendance, productivity, quality, customer satisfaction, and operational performance.

# KPIs
Total Calls, 
Total Cases Worked, 
SOlve Rate, 
Avg CSAT, 
Avg Quality Score, 
Attendence %, 
Aux %

# Dashboard Screenshots
**EXECUTIVE SUMMARY**
<img width="1382" height="813" alt="image" src="https://github.com/user-attachments/assets/48b7a4dc-137b-4239-8f47-c6a692627ccd" />
**AGENT PERFORMANCE**
<img width="1380" height="810" alt="image" src="https://github.com/user-attachments/assets/848a5434-afa9-44b1-9b93-4cbeb2fcd401" />
**OPERATIONS ANALYSIS**
<img width="1383" height="809" alt="image" src="https://github.com/user-attachments/assets/b6b46ed3-c76f-4e52-8b25-e2439585634e" />
**QUALITY ANALYSIS**
<img width="1376" height="808" alt="image" src="https://github.com/user-attachments/assets/819ef679-74a8-40ca-abf8-966b0c3687a6" />
**CUSTOMER SATISFACTION**
<img width="1380" height="808" alt="image" src="https://github.com/user-attachments/assets/9db7c3fd-ea7c-4ff2-bcaa-b09b00646057" />

# Business Insights
**EXECUTIVE SUMMARY INSIGHTS:**
• Call volume shows noticeable fluctuations with intermittent peak days, indicating inconsistent demand patterns.
• The overall solve rate is around 60%, highlighting a clear opportunity to improve resolution efficiency.
• Case resolution is concentrated among a smaller group of agents, suggesting workload imbalance.
• While attendance levels are stable, a significant portion of time is spent in auxiliary activities, which may be impacting productivity.

**AGENT PERFORMANCE INSIGHTS:**
• Certain agents demonstrate higher efficiency by resolving more cases with lower talk time.
• Some agents are handling higher call volumes but are not achieving proportional resolution rates, indicating potential performance gaps.
• There is a clear performance gap between top and low performers, suggesting the need for targeted coaching.
• Increased talk time does not consistently translate into better outcomes, indicating inefficiencies in handling time.

**OPERATIONS ANALYSIS INSIGHTS:**
• Inbound call volume consistently exceeds outbound, indicating a reactive support model.
• A considerable amount of time is categorized as unavailable or non-productive, which may impact overall operational efficiency.
• Occupancy levels vary significantly across agents, pointing to uneven workload distribution.
• Higher unavailable time for certain agents may be directly affecting team productivity and service levels.

**QUALITY ANALYSIS INSIGHTS:**
• A few ticket categories, particularly high-volume ones like faulty or damaged items, are driving the majority of workload.
• While solve rates appear strong across categories, they should be evaluated alongside volume to ensure balanced performance.
• Some categories may require faster resolution cycles to improve overall service efficiency.

**CUSTOMER SATISFACTION INSIGHTS:**
• Customer ratings are largely positive, with most responses skewed toward higher scores.
• However, even a small proportion of low ratings can have a noticeable impact on overall CSAT.
• Certain agents consistently achieve higher CSAT scores, indicating best practices that can be replicated.
• Variations in CSAT across brands suggest differences in service experience that may require further investigation.
