# PhonePe Transaction Analytics Dashboard \| Power BI

An interactive Power BI dashboard built to explore PhonePe transaction
performance, monthly trends, service-level activity, customer segments,
and transaction behavior. The project focuses on turning transaction
data into clear, business-friendly insights using data modeling, DAX
measures, KPI cards, and visual analysis.

> **Tools:** Power BI Desktop · DAX · Power Query · Data Modeling · Data
> Visualization

------------------------------------------------------------------------

## Dashboard Preview

![PhonePe Transaction Analytics Dashboard](assets/phonepe-dashboard.png)

> **Add your screenshot:** Create an `assets` folder in this repository,
> save your final Power BI dashboard screenshot as
> `phonepe-dashboard.png`, and commit it. The image will appear here
> automatically on GitHub.

------------------------------------------------------------------------

## Project Objectives

-   Monitor high-level transaction KPIs in one place.
-   Analyze transaction value trends by month.
-   Compare transaction activity across services.
-   Identify high-volume customer names and age segments.
-   Compare weekday and weekend transaction behavior.
-   Present key metrics in a clean, interactive dashboard.

## Key Dashboard Metrics

The current dashboard displays the following headline metrics:

  ------------------------------------------------------------------------
  KPI                                Displayed value What it tells us
  --------------------- ---------------------------- ---------------------
  Total Transaction                       **3.47bn** Overall transaction
  Value                                              value represented in
                                                     the dashboard

  Total Transactions                        **300K** Total transaction
                                                     volume

  Success Rate                            **96.00%** Share of transactions
                                                     marked successful,
                                                     based on the model's
                                                     definition

  Total Users                               **108K** Total users
                                                     represented in the
                                                     report

  Transaction Value MoM                    **8.98%** Month-over-month
                                                     change in transaction
                                                     value

  Transaction MoM                          **8.97%** Month-over-month
                                                     change in transaction
                                                     volume
  ------------------------------------------------------------------------

*These values reflect the current dashboard view. Confirm the reporting
period, currency/unit, and measure definitions in Power BI before
publishing.*

------------------------------------------------------------------------

## Key Insights

Based on the visuals and values currently shown in the dashboard:

1.  **Transaction value is 3.47bn.** This provides a high-level view of
    the total value flowing through the transactions represented in the
    report.
2.  **Transaction volume is 300K.** This gives a quick view of activity
    across the selected reporting period.
3.  **The displayed success rate is 96%.** The remaining share can be
    investigated by reviewing failed, pending, or otherwise unsuccessful
    transactions, depending on the dataset's status categories.
4.  **Month-over-month indicators are positive.** The dashboard displays
    8.98% for transaction value MoM and 8.97% for transaction MoM.
    Validate the comparison months and DAX logic before using these
    figures in business decisions.
5.  **Loans lead the service comparison in the displayed chart.**
    Insurance and Money Transfer follow, while Recharge Bills has the
    smallest bar in the current view.
6.  **Weekday activity is higher than weekend activity in the displayed
    breakdown.** The chart shows approximately 249.4K (83.4%) for
    weekdays and 61.2K (21.6%) for weekends. These percentages total
    105%; review the underlying measures, denominator, and labels before
    treating the split as final.
7.  **The age-segment visual supports customer segmentation.** Use it to
    compare the distribution of users across Gen X, Millennials, Gen Z,
    and Boomers, and validate the segment totals against the source
    data.

### Business Questions This Dashboard Helps Explore

-   How are transaction value and transaction count changing over time?
-   Which services contribute the most transaction value?
-   Is transaction activity different on weekdays versus weekends?
-   Which customer segments account for a larger share of users?
-   Is the transaction success rate meeting the desired target?
-   Are month-over-month changes consistent across value and volume?

------------------------------------------------------------------------

## Problem Statement

Transaction data can be difficult to interpret when important measures
are spread across tables or separate reports. Without a consolidated
view, it takes more time to monitor transaction performance, compare
services, understand customer segments, and spot changes over time.

## Solution

This project brings the main transaction KPIs and supporting visuals
into a single Power BI report. KPI cards summarize performance, trend
charts show changes over time, service comparisons highlight differences
between categories, and donut charts help compare weekday/weekend
activity and age segments. The dashboard is designed to make exploration
faster and support data-informed questions.

## Dashboard Components

-   **KPI cards:** Total Transaction Value, Total Transactions, Success
    Rate, and Total Users.
-   **Monthly trend:** Total Transaction Value by Month.
-   **MoM indicators:** Transaction Value MoM% and Total Transactions
    MoM%.
-   **Service comparison:** Total Transaction Value by Service.
-   **Name comparison:** Total Transaction Value by Name.
-   **Weekend analysis:** Total Transactions by Weekday/Weekend.
-   **Age segmentation:** Count of User_ID by Age Segment.
-   **Month filter:** Allows users to explore the available reporting
    months, where supported by the model.

## Data Preparation & Modeling

The report was built as a practice project to apply a BI workflow:

1.  Load the source transaction data into Power BI.
2.  Inspect column names, data types, missing values, and duplicate
    records.
3.  Clean and transform data in Power Query where needed.
4.  Build relationships and a data model appropriate to the source
    tables.
5.  Create DAX measures for the headline KPIs and month-over-month
    comparisons.
6.  Build and format the visuals, then validate totals against the
    source data.

> Update this section to match the exact transformations, relationships,
> and DAX measures used in your final `.pbix` file.

## Challenges & Solutions

  -----------------------------------------------------------------------
  Challenge                           Approach / solution
  ----------------------------------- -----------------------------------
  Many metrics need to fit on one     Grouped KPIs and charts into a
  page                                clear visual hierarchy

  Comparing performance over time     Used a monthly trend chart and MoM
                                      measures

  Comparing services and customer     Used bar and donut charts suited to
  groups                              category comparisons

  Keeping the report visually         Applied a unified PhonePe-inspired
  consistent                          purple theme, consistent spacing,
                                      and aligned visual containers

  Ensuring metrics are trustworthy    Validate DAX measures, reporting
                                      periods, denominators, and chart
                                      totals against the source data
  -----------------------------------------------------------------------

## What I Learned

-   Creating and formatting an interactive Power BI report.
-   Writing and applying DAX measures for KPI calculations and MoM
    analysis.
-   Organizing data and relationships for reporting.
-   Choosing charts based on the question being answered.
-   Building a consistent dashboard layout and visual hierarchy.
-   Checking totals and percentage calculations before presenting
    insights.

## Repository Structure

``` text
phonepe-transaction-analytics/
├── README.md
├── assets/
│   └── phonepe-dashboard.png
└── PhonePe-Transaction-Analytics.pbix
```

Use your actual `.pbix` filename if it differs. Add the source dataset
only if you are allowed to share it and it contains no sensitive
information.

## How to View the Project

1.  Download or clone this repository.
2.  Open `PhonePe-Transaction-Analytics.pbix` in Power BI Desktop.
3.  Refresh the data source if required and available.
4.  Use the report filters to explore the dashboard.

## Future Improvements

-   Add a dedicated transaction-status analysis to investigate
    unsuccessful transactions.
-   Validate and standardize all percentage calculations and KPI units.
-   Add drill-through pages for service, region, and customer-segment
    analysis if the dataset supports them.
-   Improve tooltip details and add contextual explanations for key
    metrics.
-   Add a data dictionary documenting the important columns and DAX
    measures.

## Disclaimer

This is an analytics portfolio project. The displayed metrics and
observations describe the current report view and should not be
interpreted as official PhonePe company results. Any business
conclusions should be verified against the original data, metric
definitions, and reporting period.

------------------------------------------------------------------------

**Author:** Your Name\
**Project:** PhonePe Transaction Analytics Dashboard\
**Built with:** Microsoft Power BI
