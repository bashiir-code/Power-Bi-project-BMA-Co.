# Power-Bi-project-BMA-Co.

(Sales - Gross Profit - Quantity) Performance Dashboard Project
-------------------------------------------------------------------
Objective
----------

The purpose of this dashboard is to analyze and compare YTD (Year-to-Date) and PYTD (Prior Year-to-Date) (Sales - Gross Profit - Quantity) across  2023 and 2024. The dashboard enables stakeholders to monitor performance trends and identify key areas for improvement.

2022 serves as the PYTD reference for 2023's YTD.

2023 serves as the PYTD reference for 2024's YTD.

This comparison helps evaluate growth or decline in absolute (Sales - Gross Profit - Quantity) figures.




Data Preparation in Power Query:
-------------------------------

Imported raw (Sales - Gross Profit - Quantity) data for 2022, 2023, and 2024.

Transformed the data by:

Promoting headers for easier interpretation.

Changing data types for consistency.

Removing duplicates to ensure data accuracy.

Renaming columns for clarity.

![Screenshot 2025-01-04 133047](https://github.com/user-attachments/assets/db45c2e4-cc6a-4042-a2dd-5ab4c763d53d)



Created a DimDate Table:
-----------------------

Designed a custom date dimension table to handle partial-year data for 2024.

Included fields such as Year, Month, Quarter, and Day to enable detailed time-based filtering and analysis.

Ensured compatibility with YTD and PYTD calculations by mapping dates across years.

![image](https://github.com/user-attachments/assets/d983058c-f225-4790-aae5-20789a794000)




Created Additional Dimension and Measure Tables:
-----------------------------------------------
Slc_Dim: A slicer table for filtering by (Sales - Gross Profit - Quantity), Gross Profit and Quantity.

![image](https://github.com/user-attachments/assets/e12485a1-e0ca-4254-ab7a-cbdea460ce37)


Measure Table: Defined critical metrics, including:

![image](https://github.com/user-attachments/assets/0a461403-571c-4d2d-a6d4-a0d784ed1dc2)



YTD (Sales - Gross Profit - Quantity): Cumulative (Sales - Gross Profit - Quantity) for the current year up to the latest available date.

PYTD (Sales - Gross Profit - Quantity): Cumulative (Sales - Gross Profit - Quantity) for the same period in the prior year.

YTD vs PYTD: Difference between YTD and PYTD (Sales - Gross Profit - Quantity).

Defined Relationships:
---------------------
Established relationships between fact and dimension tables to ensure accurate filtering and calculations.

![image](https://github.com/user-attachments/assets/164a07ec-0f38-4bd9-8553-79cd16965e1b)



Dashboard Creation:
-------

Designed the dashboard with visuals that compare (Sales - Gross Profit - Quantity) across 2022, 2023, and 2024:

![image](https://github.com/user-attachments/assets/1b8c5cd5-2e4e-4a46-b4e1-acf29a764a41)


This Line and Stacked Column Chart compares the Year-to-Date (YTD) (Sales - Gross Profit - Quantity) of the current year (2024) to the Prior Year-to-Date (PYTD) (Sales - Gross Profit - Quantity) of the previous year (2023) and (2023) to (2022). It provides a clear month-by-month view of cumulative (Sales - Gross Profit - Quantity) trends and performance differences.

![image](https://github.com/user-attachments/assets/cde88466-b8c5-48b3-9c97-fa4574b4eb9b)


This scatter chart visualizes accounts based on their YTD Value (X-Axis) and Gross Profit Percentage (GP%) (Y-Axis). The goal is to segment accounts and identify which ones the company should prioritize for focus.

![image](https://github.com/user-attachments/assets/57ae6eaa-0c18-40d8-bfd8-fe9601a1a631)



This Treemap highlights the 10 countries with the lowest (Sales - Gross Profit - Quantity) across the dataset.
Helps focus on areas requiring strategic attention.

![image](https://github.com/user-attachments/assets/f0f89158-b218-4cb3-afe1-512f2e398ae3)


This waterfall chart visualizes the difference between YTD (Year-to-Date) and PYTD (Previous Year-to-Date) over time, helping to identify trends in performance changes. It supports drill down

Filters and Slicers:
------------------

Allow users to explore data interactively by filtering by year, region, or product category.

Dashboard
--

![Screenshot 2025-01-04 132625](https://github.com/user-attachments/assets/3d768239-283e-4b53-b083-078d69037ec5)




Key Insights
------

YTD vs. PYTD (Sales - Gross Profit - Quantity):

2024 vs. 2023: YTD (Sales - Gross Profit - Quantity) for 2024 are compared against PYTD (Sales - Gross Profit - Quantity) from 2023.

2023 vs. 2022: YTD (Sales - Gross Profit - Quantity) for 2023 are compared against PYTD (Sales - Gross Profit - Quantity) from 2022.

This provides a clear view of how (Sales - Gross Profit - Quantity) have grown or declined in absolute numbers.
Seasonality and Trends:

Monthly trends reveal consistent (Sales - Gross Profit - Quantity) spikes during specific months across years.

Declines in certain months point to potential challenges or opportunities for improvement.

Underperforming Regions:
----
The bottom 10 countries analysis identifies areas with low (Sales - Gross Profit - Quantity) performance.
This insight can guide targeted marketing and operational efforts.
Partial-Year Analysis:

The custom DimDate table enabled accurate comparisons despite 2024 being a partial year.
The dashboard ensures that comparisons between YTD and PYTD are aligned correctly.
