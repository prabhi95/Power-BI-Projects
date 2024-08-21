
# Finance-Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/aea4e4c9-1ca8-4a19-88ae-38a183d9422b/36750db7a63271640754?experience=power-bi

## Problem Statement
**Objective:**  
The organization needs a centralized and dynamic tool to monitor and analyze the financial performance of its sales teams across different time periods. Currently, there is a lack of visibility into how individual salespeople and teams are performing against their monthly targets, as well as the overall financial performance trends. This makes it challenging to identify areas of improvement, make informed decisions, and communicate performance insights to stakeholders.

**Challenges:**
- The current process of tracking sales performance is manual and time-consuming, relying on static reports that do not provide real-time insights.
- There is a need to compare actual sales figures against targets to understand variances, identify trends, and determine the effectiveness of sales strategies.
- Management requires a clear and visually intuitive way to assess whether monthly and year-to-date (YTD) targets are being met, both at the individual and team levels.
- The existing reports lack interactivity, making it difficult to drill down into specific data points or customize the view according to different analysis needs.

**Desired Outcome:**
To address these challenges, a finance KPI dashboard will be developed in Power BI. The dashboard will:
- Provide real-time tracking of actual sales performance against set targets.
- Highlight key performance indicators (KPIs) such as total sales, variances, and target achievement rates.
- Enable drill-down capabilities for detailed analysis at the team and individual levels.
- Present the data in an interactive, visually engaging format that supports informed decision-making and strategic planning.

---
## **Steps followed**
1. **Data Preparation**: Data for the dashboard was prepared using four different tables. The actual performance table outlined each salesperson's monthly performance in a pivot report style, and a similar table provided monthly targets for each salesperson. A simplified calendar table for the analysis period and a People Dimension table for team details were also included. These worksheets were loaded into Power Query for transformation. The first row was promoted as headers, and the actual and target tables were unpivoted to create standard three-column tables for easier analysis. Columns were renamed, and appropriate data types were set. Additional columns were added to the calendar table using the "Add Column" ribbon for quick analysis once the data was loaded into Power BI.

2. **Data Modeling**: After loading the tables into Power BI, data modeling was conducted by connecting the tables in the model view. The actual and target tables served as fact tables and were joined via date columns. The model was organized to centralize the fact tables and place dimensions on the sides, setting the foundation for accurate calculations and visualizations.

3. **DAX Calculations**: Key financial performance indicators (KPIs) were defined using DAX calculations. These included total sales (actual and target), variance, and variance percentage. Year-to-date (YTD) values were calculated, and a measure was created to count the months where targets were met. These measures enabled dynamic analysis at both the overall and individual levels, providing insights into performance trends.

4. **Dashboard Design**: The finance KPI dashboard was designed with a custom theme to ensure visual consistency. The dashboard was divided into three sections: a summary of all finance KPIs, a detailed view, and a section for filters and slicers. Card visuals were used for the main KPIs, with reference labels for YTD values. A win/loss chart visually represented target achievement each month, and a trend chart displayed actual versus target performance over time.

5. **Enhancements and Final Touches**: A DAX measure was created to transform variance percentages into a visual representation using emojis, enhancing engagement. Visuals were refined, conditional formatting was added, and a dynamic title was introduced based on slicer selections. A table visual displaying team-level performance, including images, data bars, and sparkline trends, was also added.

6. **Smart Narrative and Finishing Touches**: A smart narrative visual was added to generate dynamic commentary based on the data, making the dashboard more insightful. The report was polished by adding a corporate logo, a red accent bar, and adjusting slicer settings, resulting in an elegant and comprehensive overview of financial performance.

7. **Report Publishing**: After completing the dashboard, the final report was published to the Power BI service. This allowed for easy sharing and collaboration across the team, ensuring that stakeholders could access real-time insights and make data-driven decisions.

## Snapshot of Dashboard

![1724226788360-487eb6ce-8ffb-481c-a3f9-9deb6b3e9c82_1](https://github.com/user-attachments/assets/6249e26b-0389-4327-bb71-0a6a2292ab05)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

1. **Overall Sales Performance**:
   - The total sales actual is **$18.9M** compared to a target of **$19.3M**, resulting in a negative variance of **($366.9K)**.
   - Year-to-date (YTD) figures show total sales actual at **$2.4M** against a target of **$2.6M**, reflecting a negative YTD variance of **($112.7K)**.
   - The variance percentage indicates a shortfall of **4.4% YTD**.

2. **Monthly Performance**:
   - Sales targets were met in only **2 out of 14 months**, indicating a consistent challenge in achieving sales goals.
   - Specific months, such as May and September 2023, showed stronger performance with variances of **5.5%** and **3.4%** respectively.
   - Conversely, months like November 2023 and January 2024 saw significant shortfalls, with variance percentages of **(-8.2%)** and **(-4.2%)**.

3. **Salesperson Analysis**:
   - Among the sales team, **Gunnar Cockshoot** and **Barr Faughny** are the top performers, with actual sales figures of **$846.5K** and **$808.1K** respectively.
   - However, many salespeople have not met their targets, as indicated by negative variance percentages, with **Van Tuxwell** having a particularly large shortfall of **(-6.7%)**.
   - The status indicators and trend analysis suggest that some team members are consistently underperforming, potentially requiring attention or support.

4. **Engagement and Visual Insights**:
   - The smart narrative and use of emojis in the status column provide a quick, engaging summary of the performance data.
   - The dashboard effectively communicates the need for strategic adjustments to meet targets, highlighting months and individuals that are falling short of expectations.

