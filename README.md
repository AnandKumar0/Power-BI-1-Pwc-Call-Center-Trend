# Call Center Data Analysis using Power BI

## Project Overview

**Project Title:** Call Center Trends – Overview Dashboard

**Tool Used:** Power BI Desktop

**Data Source:** Call Center Dataset (CSV, 5000 records)

This project demonstrates data visualization and dashboarding skills commonly used by Data Analysts to transform raw call center data into actionable business insights. It replicates a real-world call center performance monitoring scenario, covering agent performance, customer satisfaction, call resolution, and call volume trends.

The project covers the complete BI workflow, including data cleaning, data modeling, DAX measure creation, and interactive dashboard design with slicers for dynamic filtering.

## Objectives

**Data Cleaning & Preparation**
Import and clean the raw call center CSV data — handling inconsistent time formats, blank columns, and categorical fields (answered/resolved flags) before loading into the data model.

**Data Modeling**
Structure the dataset for efficient DAX calculations, including derived fields such as day of week, hour of call, and satisfaction level buckets.

**KPI Design**
Build key performance indicator cards to summarize overall call center health at a glance (total calls, resolve %, abandon %, answer speed, handling time, satisfaction).

**Interactive Dashboarding**
Design a single-page interactive overview report with slicers (Agent, Topic, Month, Week Day) enabling stakeholders to drill down into specific segments.

**Business Analysis**
Answer real-world business questions covering agent performance, customer satisfaction distribution, and call volume patterns by hour and day.

## Data Quality Checks

Before building the model, the raw data was reviewed for:

- **Missing values** — blank/unanswered calls where speed of answer and talk duration were not applicable
- **Data type consistency** — converting time fields and satisfaction ratings into usable numeric/date formats
- **Categorical standardization** — ensuring answered/resolved flags and topic categories were consistent for accurate aggregation
- **Duplicate call IDs** — verified each call id is unique

## Dashboard Structure

### Page: Call Center Trends – Overview

**KPI Cards**
- Total Calls: 5,000
- Customer Satisfaction: 68.07%
- Call Resolve %: 89.94%
- Call Abandoned %: 18.92%
- Call Answered Speed (avg, seconds): 67.52
- Avg Call Handling Time: 224.92

**Agent Performance Table**
Breaks down Total Calls, Call Abandon %, Answered Speed, Call Resolve %, and Satisfaction by individual agent (Becky, Stewart, Diane, Jim, Dan, Greg, Martha, Joe) — used to identify top and underperforming agents.

**Total Calls by Satisfaction Level**
Bar chart segmenting all calls into satisfaction buckets: Not Served, Very Dissatisfied, Dissatisfied, Normal, Satisfied, Very Satisfied.

**Hourly Calls**
Line chart showing call volume distribution across operating hours (09:00–18:00) — used to identify peak call hours for staffing decisions.

**Days Wise Calls**
Line chart showing call volume by day of week (Mon–Sun) — used to identify the busiest days.

**Slicers / Filters**
- Agent
- Topic
- Month Name
- Week Day
- Clear Filters button (resets all slicers)

**Other Elements**
- Last Call Received (card showing timestamp of most recent call)

## Findings

- **Agent Performance** — Answered speed and satisfaction vary noticeably across agents (Becky's answered speed of 65.33s vs Joe's 70.99s), highlighting coaching opportunities.
- **Call Abandonment** — Nearly 1 in 5 calls (18.92%) are abandoned, indicating a queue/staffing gap during peak periods.
- **Satisfaction Distribution** — The majority of calls fall into "Normal" and "Satisfied" buckets, but a meaningful share (Not Served + Very Dissatisfied + Dissatisfied) represents a churn/reputation risk.
- **Peak Hours** — Call volume peaks around 11:00 and again in the afternoon, useful for shift planning.
- **Peak Days** — Monday and Saturday see the highest call volumes, while Tuesday is consistently the quietest.

## Conclusion

This project helped strengthen practical Power BI and DAX skills for building executive-ready dashboards from operational data. It demonstrates practical experience in:

- Cleaning and modeling raw operational data
- Building meaningful KPIs for stakeholder reporting
- Designing an interactive, filterable single-page dashboard
- Deriving actionable business insights from call center metrics

The insights generated from this dashboard can support decision-making related to agent coaching, staffing/shift planning, and customer satisfaction improvement initiatives.

## How To Use

1. Download or clone this repository.
2. Open `Call_Center_Dashboard.pbix` in Power BI Desktop.
3. If prompted, update the data source path to point to `01_Call-Center-Dataset.csv` on your local machine.
4. Refresh the data model.
5. Explore the dashboard using the Agent, Topic, Month, and Week Day slicers.

## Author

**Anand Kumar**
PostgreSQL | Excel | Adv Excel

Power BI | DAX | Data Analytics

This project is part of my Data Analytics portfolio showcasing Power BI dashboarding skills required for Data Analyst roles.

Feel free to connect, provide feedback, or collaborate on future projects.
