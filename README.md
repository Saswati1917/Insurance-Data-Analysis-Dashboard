# Insurance-Data-Analysis-Dashboard
End-to-end Power BI project on Insurance Data Analysis — SQL Server (data source), Power Query (ETL), DAX (measures), RLS (security), and interactive dashboard with KPIs for premiums, claims, and customer demographics.

**Problem Statement**

The objective of this project was to analyse insurance policy and claims data to help Prism Insurance Pvt. Ltd. track performance across policies, claims, and customer demographics.

**The dashboard provides:**

1. Financial KPIs such as Premiums, Coverage, and Claim Amounts.

2. Policy activity monitoring (Active vs Inactive).

3. Claims breakdown by status, policy type, and customer demographics.

This enables management to identify business drivers, claim bottlenecks, and high-risk customer segments in one unified view.

**Steps Followed**

Step 1: Loaded the dataset (CSV) into the SQL Server database insuranceDB.

Step 2: Connected Power BI Desktop to SQL Server in Import Mode.

Step 3: Performed data profiling (column distribution, quality, profile for full dataset).

Step 4: Cleaned and transformed data in Power Query:

1. Created Age Group column (Young Adult, Adult, Elder).

2. Created Policy Status column (Active/Inactive based on end date).

Step 5: Built DAX measures for KPIs (Premium Amount, Coverage Amount, Claim Amount).

Step 6: Designed report visuals:

1. Cards for KPIs

2. Slicers for Policy, Claim, Customer ID

3. Ribbon chart for Claim Status

4. Bar chart for Premium by Policy Type

5. Line chart for Claim Amount by Age Group

6. Donut chart for Active vs Inactive policies

7. Matrix for Claim Amount by Policy Type & Claim Status

Step 7: Applied a dark theme with consistent formatting for readability.

Step 8: Implemented Row-Level Security (RLS) for Health & Travel policy managers.

Step 9: Published the report to Power BI Service, created a workspace, and built a dashboard by pinning visuals.

Step 10: Configured personal gateway and scheduled daily data refresh.

**Tech Stack & Tools Used**

Database: Microsoft SQL Server

ETL & Data Preparation: Power Query (in Power BI)

Data Modelling & Measures: DAX (Data Analysis Expressions)

Visualisation: Power BI Desktop

Collaboration & Deployment: Power BI Service (workspace, dashboards, sharing)

Data Refresh: Personal Gateway + Scheduled Refresh

**Insights**

🔑 Key KPIs

Premium Amount: 5.98M

Coverage Amount: 600.55M

Claim Amount: 16.91M

📌 Policy Status

Active Policies: 5.82K (58.13%)

Inactive Policies: 4.19K (41.87%)

📊 Premium by Policy Type

Travel: 2.5M (highest)

Health: 1.2M

Auto: 1.0M

Life: 0.7M

Home: 0.6M

👉 Travel insurance is the strongest business line by premium collection.

📌 Claim Status

Rejected: 4.4K (highest)

Settled: 3.4K

Pending: 2.3K

👉 A high rejection rate could indicate fraud detection or customer dissatisfaction.

👥 Customer Demographics

Male: 5,003

Female: 5,001 → Gender split is nearly equal.

👤 Claim Amount by Age Group

Adults: 8.6M (highest)

Elders: 6.4M

Young Adults: 1.9M (lowest)

👉 Adults (26–60 years) are the most high-risk group with the largest claim payouts.

📌 Claim Amount by Policy Type (Matrix)

Health policies → highest pending claims (~27.68M)

Travel policies → highest rejected claims (~103.96M)

Health + Travel dominates both pending and rejected categories.

**Business Takeaways**

1. Travel policies generate maximum premium revenue, but also face the highest claim rejections.

2. Health policies account for the largest pending claim amounts → potential delays in processing.

3. Adults are the most high-risk segment, aligning with expected risk exposure.

4. Customer base is evenly split across genders, avoiding bias.

5. Majority of policies are active (58%), reflecting strong retention.

**How to Use**

1. Open the dashboard link in Power BI Service.

2. Use slicers to filter by Policy Number, Claim Number, or Customer ID.

3. Hover or click visuals for cross-filtering and drill-through.

4. Use the dashboard view in Power BI Service for quick KPI monitoring.
