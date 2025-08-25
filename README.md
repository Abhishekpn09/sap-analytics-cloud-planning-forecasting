SAP Analytics Cloud – Planning & Forecasting Project

This repository documents my hands-on project with SAP Analytics Cloud (SAC), where I designed planning models, performed forecasting simulations, and developed interactive stories.

The goal of this project was to understand how SAC can be used for enterprise planning workflows, from data modeling to predictive forecasting and visualization.

🔧 Technical Implementation
1. Planning Models

Defined dimensions:

Product Group (Bikes, Accessories, Touring, Mountain, Trend)

Account (Revenue, Quantity, Statistical KPIs)

Time (2015–2022, monthly granularity)

Version (Actuals, Plan, Forecast, Rolling Forecast)

Added measures: Revenue (LC), Quantity.

Configured private/public dimensions and hierarchies.

Managed master data and loaded transactional data (2015–2021 actuals).

2. Central Planning Functions

Used SAC’s built-in functions to simulate real-world business planning workflows:

Version Management: Created private forecast versions (FCV1, FCV2, FCV4) → published to public versions after validation.

Variance Analysis: Compared Plan vs. Forecast vs. Actual revenue across product groups.

Mass Data Entry & Disaggregation: Adjusted values top-down (e.g., corporate sales targets) and allocated across product hierarchies.

Data Actions: Built reusable scripts for copying data, allocations, and running transformations.

Currency Conversion: Defined conversion tables to simulate revenue impact across local and global currencies.

3. Forecasting & Predictive Analytics

Applied Predictive Forecasts directly in SAC stories using historical sales data.

Built Value Driver Trees (VDTs) to model business dependencies:

Nodes represented drivers (marketing spend, product demand) and outcomes (revenue).

Ran what-if scenarios (e.g., increase marketing by 10%) to measure KPI impact.

Developed a Rolling Forecast for Mountain Bikes:

Monthly forecast from July–Nov 2021.

Compared Actuals vs. Forecast Versions (FCV4).

Showed cut-over to Jan 2022 as Forecast baseline.

4. Stories (Dashboards)

Built interactive dashboards (Stories) as the front-end for business users:

Sales_Planning_Story_SAC.pdf

Visualized historical sales data (2015–2021) by Product Group.

Displayed both quantity and revenue KPIs.

Enabled comparison of actuals vs. planned versions.

Value_Driver_Tree_Story_SAC.pdf

Implemented SAC’s Value Driver Tree widget.

Allowed interactive scenario simulations for sales forecasting.

Showed dependencies between input drivers and revenue impact.

Rolling_Forecast_Story_SAC.pdf

Designed for Mountain Bikes sales.

Included monthly rolling forecasts with version filters.

Integrated predictive outputs into planning models.

🏗️ Workflow Overview
[Data Sources: Historical Sales (2015–2021)]
          ↓
 [Planning Model in SAC]
   - Dimensions: Product, Account, Time, Version
   - Measures: Revenue, Quantity
          ↓
 [Central Planning Functions]
   - Mass Data Entry
   - Variance Analysis
   - Data Actions & Currency Conversion
          ↓
 [Forecasting Layer]
   - Predictive Forecast (time-series)
   - Value Driver Trees (scenario simulation)
   - Rolling Forecast (monthly updates)
          ↓
 [Stories / Dashboards]
   - Sales Planning Story
   - Value Driver Tree Story
   - Rolling Forecast Story

📂 Repository Contents

Sales_Planning_Story_SAC.pdf – Story on sales planning with historical data and revenue/quantity trends by product group.

Value_Driver_Tree_Story_SAC.pdf – Story showcasing the use of Value Driver Trees for sales forecasting and scenario analysis.

Rolling_Forecast_Story_SAC.pdf – Story implementing a rolling forecast for Mountain Bikes with monthly breakdown and version comparisons.

🚀 Key Takeaways

This project demonstrates how SAP Analytics Cloud supports:

✅ End-to-End Planning: From data modeling to forecasting and reporting.

✅ Predictive Analytics: Using built-in forecasting and driver-based models.

✅ Collaboration & Storytelling: Enabling interactive dashboards for business users.

By combining planning models, forecasting techniques, and stories, I simulated real-world financial & sales planning workflows in SAC.
