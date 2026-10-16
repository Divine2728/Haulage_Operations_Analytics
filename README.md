# Haulage Operations Analytics Dashboard | Excel & Power BI

## Project Overview

This project focuses on analyzing haulage and transportation operations for H&R Haulverge Ltd using Microsoft Excel and Power BI.

Developed as part of the **CodeAlpha Data Analytics Internship**, the project transforms raw operational data into a structured analytical dataset and an interactive executive dashboard.

The analysis examines trip performance, transportation costs, fuel consumption, maintenance expenditure, route activity, and delivery reliability. The goal is to demonstrate how data cleaning, exploratory analysis, and visualization can help organizations understand operational performance and make more informed decisions.

## Project Objectives

- Clean and standardize raw haulage records for reliable analysis.
- Evaluate trip volume, total distance, and transported quantities.
- Analyze transportation expenditure and its major cost components.
- Examine fuel efficiency and fuel costs relative to distance travelled.
- Compare trip statuses and investigate delivery reliability.
- Identify monthly patterns in trip activity and operating costs.
- Compare route performance and identify areas for further investigation.
- Develop an interactive Power BI dashboard for operational monitoring and decision support.

## Tools and Technologies

- **Microsoft Excel:** Data cleaning, transformation, calculated columns, pivot tables, and exploratory analysis.
- **Microsoft Power BI:** Interactive dashboard development, KPI visualization, and operational reporting.
- **Data Visualization:** KPI cards, doughnut charts, bar charts, line charts, and route comparisons.

## Dataset Overview

The Excel workbook contains raw data, cleaned data, cleaning notes, business questions, and supporting pivot tables.

The cleaned dataset contains **100 unique trip records** covering January to September 2025.

The dataset includes information on:

- Trip IDs and dates
- Truck IDs and vehicle registration numbers
- Drivers
- Origin and destination
- Departure and arrival times
- Distance travelled and trip duration
- Goods transported and quantity
- Fuel consumption and fuel expenditure
- Driver allowances and toll costs
- Maintenance expenditure
- Total trip costs
- Trip status and on-time delivery indicators

## Data Cleaning and Preparation

Data preparation was performed in Microsoft Excel to improve consistency and support reliable analysis.

The documented cleaning procedures included:

1. **Text standardization:** Standardizing text fields to improve consistency during filtering and aggregation.
2. **Date and time formatting:** Formatting dates and departure and arrival times appropriately.
3. **Calculated columns:** Adding helper columns for month, fuel cost per kilometre, cost per quantity, and fuel efficiency.
4. **Maintenance classification:** Creating a maintenance flag to distinguish trips with recorded maintenance expenditure from those without it.
5. **Issue classification:** Adding an issue flag to support the investigation of potentially problematic trips.
6. **Currency formatting:** Applying appropriate currency formats to monetary fields.
7. **Pivot table analysis:** Summarizing trip counts, distance, quantity, costs, fuel efficiency, and maintenance expenditure.

The cleaned worksheet contains 100 distinct trip IDs with no duplicate trip identifiers. The on-time delivery field has 20 blank values, corresponding to trips recorded as in transit. These records should not automatically be classified as late or failed deliveries.

## Key Performance Indicators

The following figures are based on the **full cleaned dataset**, not the filtered dashboard screenshot.

| KPI | Full-dataset result |
|---|---:|
| Total Trips | 100 |
| Total Distance | 40,795 km |
| Total Quantity Transported | 33,546 |
| Total Trip Cost | ₦10,123,090 |
| Total Fuel Cost | ₦7,792,090 |
| Total Fuel Used | 8,202.2 litres |
| Total Maintenance Cost | ₦1,365,000 |
| Total Driver Allowances | ₦850,000 |
| Total Toll Costs | ₦116,000 |
| Average Fuel Efficiency | Approximately 4.97 km/L |

*Figures are taken from the cleaned dataset and supporting pivot table. Fuel efficiency is calculated as total distance divided by total fuel consumed.*

## Dashboard Features

The Power BI report presents operational indicators and visual comparisons in an executive dashboard.

### 1. Operational KPIs

The dashboard includes indicators for total trips, distance travelled, trip costs, cost per kilometre, fuel efficiency, toll expenditure, driver allowances, maintenance costs, fuel consumption, fuel expenditure, and on-time delivery rate.

These indicators provide a summary of operational activity and expenditure.

### 2. Trip Status Analysis

A doughnut chart compares the distribution of trip statuses across the recorded dataset.

| Trip Status | Number of Trips | Share of All Trips |
|---|---:|---:|
| Completed | 51 | 51% |
| Delayed | 16 | 16% |
| Failed | 13 | 13% |
| In Transit | 20 | 20% |
| **Total** | **100** | **100%** |

This breakdown helps distinguish completed journeys from delayed, failed, and ongoing trips.

### 3. Monthly Trip Trends

A monthly chart displays trip activity over time, helping users identify fluctuations in the number of recorded journeys.

### 4. Monthly Operating Costs

The dashboard compares operating costs across months. This supports the identification of high-expenditure periods and provides a starting point for investigating changes in fuel usage, maintenance, route mix, and trip volume.

### 5. Top Routes

Route comparisons help identify frequently used routes and examine how transportation activity is distributed across origin-destination pairs.

### 6. Route Cost Analysis

Route cost visuals help compare transportation expenditure across routes and identify routes that may warrant closer investigation after accounting for distance, quantity transported, and other operational factors.

### 7. Interactive Filtering

The dashboard includes a month filter and a goods-type filter, allowing users to explore selected periods and categories of transported goods.

## Key Findings from the Full Dataset

### 1. Fuel is the largest recorded cost component

Fuel expenditure totals ₦7,792,090 out of ₦10,123,090 in total trip costs.

This represents approximately **77% of total trip expenditure**.

Fuel is therefore a major area for operational monitoring. Further analysis could compare fuel costs per kilometre across trucks and routes before recommending efficiency improvements.

### 2. Maintenance is another significant cost component

Recorded maintenance expenditure totals ₦1,365,000, representing approximately 13.5% of total trip costs.

Comparing maintenance expenditure across vehicles and routes could help identify where further investigation is justified.

### 3. Delivery status requires attention

Of the 100 recorded trips, 51 are marked completed, 16 delayed, 13 failed, and 20 in transit.

The dataset therefore records 29 trips as delayed or failed. These trips could be investigated by route, driver, truck, and goods type to identify recurring patterns.

### 4. The on-time delivery rate requires a clearly defined denominator

There are 80 trips with a recorded on-time outcome: 51 marked on time and 29 marked not on time.

Among these 80 trips, the recorded on-time rate is:

**51 ÷ 80 × 100 = 63.75%, or approximately 64%.**

This explains the dashboard's displayed 64% rate when calculated from records with known outcomes. It should not be interpreted as 64% of all 100 trips being on time. The 20 in-transit trips have no recorded outcome and should be assessed separately.

### 5. Operating costs vary by month

The supporting data shows differences in monthly total trip costs. August recorded the highest monthly expenditure at ₦2,208,630 in the cleaned dataset.

This is a useful starting point for investigating whether the higher expenditure resulted from more trips, longer distances, different routes, greater fuel consumption, or maintenance requirements.

A higher monthly cost alone does not establish inefficiency; it must be considered alongside operational activity.

## Business Questions Addressed

The project was designed to investigate questions such as:

1. How many trips were recorded, and how much distance was travelled?
2. What is the total cost of haulage operations?
3. Which cost component accounts for the largest share of expenditure?
4. How efficiently is fuel being used relative to distance travelled?
5. What proportion of trips are completed, delayed, failed, or still in transit?
6. What is the recorded on-time delivery rate among trips with known outcomes?
7. How do trip volumes and costs change across months?
8. Which routes account for the most recorded activity?
9. Which routes or vehicles may warrant further cost and performance investigation?
10. How can operational reporting support better cost control and delivery monitoring?

## Business Recommendations

Based on the findings, the following actions could support further operational analysis:

- **Monitor fuel expenditure:** Compare fuel cost per kilometre and fuel efficiency across trucks and routes, accounting for distance and load differences.
- **Investigate delayed and failed trips:** Review trip records to determine whether issues are associated with specific routes, drivers, vehicles, or goods types.
- **Review maintenance expenditure:** Compare maintenance costs across vehicles and examine whether repeated maintenance events are associated with specific operational conditions.
- **Improve delivery-status tracking:** Record delivery outcomes consistently and distinguish completed, delayed, failed, and in-transit journeys.
- **Investigate high-cost months:** Compare monthly expenditure against trip volume, distance, fuel use, and maintenance activity before drawing conclusions about cost efficiency.
- **Standardize performance monitoring:** Use consistent KPI definitions and reporting periods to support meaningful comparisons over time.

These recommendations identify areas for investigation. Additional evidence is needed before attributing the observed results to specific causes.

## Dashboard Scope and Data Validation

The Power BI screenshot is a visual preview of the report, but its displayed figures do not match the full-dataset totals in the Excel workbook.

For example, the screenshot displays 11 trips and approximately ₦958.29K in total trip costs, whereas the full cleaned dataset contains 100 trips and ₦10,123,090 in total costs.

These figures should be treated as different reporting scopes until the dashboard filters and data model have been verified. The full-dataset KPIs and findings in this README are based on the cleaned Excel worksheet and its supporting pivot table.

## Project Files

The repository is organized around the following deliverables:

- `README.md` — Project overview, methodology, findings, and recommendations.
- `Haulage_Operations_Data.xlsx` — Excel workbook containing the raw data, cleaned data, cleaning notes, business questions, and supporting pivot tables.
- `Haulage_Executive_Dashboard.pbix` — Interactive Power BI report.
- `Haulage_Dashboard_Preview.png` — Screenshot preview of the dashboard.

*Update these filenames if the files in the GitHub repository use different names.*

## Skills Demonstrated

- Data cleaning and preparation in Excel
- Exploratory Data Analysis (EDA)
- Calculated columns and KPI development
- Pivot table analysis
- Transportation and logistics analytics
- Cost and fuel efficiency analysis
- Operational performance monitoring
- Power BI dashboard design
- Data visualization and storytelling
- Evidence-based business recommendations

## Conclusion

The Haulage Operations Analytics Dashboard demonstrates how raw transportation records can be transformed into structured information for operational monitoring and decision support.

By analyzing trip activity, fuel expenditure, maintenance costs, route performance, and delivery status, the project highlights areas where a haulage business can investigate operating costs and improve the quality of its performance reporting.

Developed as part of the CodeAlpha Data Analytics Internship, this project reflects my practical application of Excel and Power BI to a real-world-style business analytics problem.

---

**Project:** Haulage Operations Analytics Dashboard  
**Organization:** H&R Haulverge Ltd  
**Programme:** CodeAlpha Data Analytics Internship  
**Tools:** Microsoft Excel and Microsoft Power BI  
**Domain:** Transportation and Logistics Analytics  
**Analysis Period:** January–September 2025
