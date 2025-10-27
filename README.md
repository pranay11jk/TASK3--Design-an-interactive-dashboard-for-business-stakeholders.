Power BI Dashboard Project — Call Center Performance Analysis
📁 Project Overview

This project analyzes call center performance using Power BI.
The dataset includes call records, agent details, product sales, and call duration metrics.
The goal is to design an interactive dashboard to monitor agent performance, call outcomes, and overall conversion efficiency.

🧩 Dataset Information

Columns Used:

Column Name	Description
AgentID	Unique identifier for each agent
CallID	Unique identifier for each call
CustomerID	Identifier for the customer contacted
PickedUp	Whether the customer picked up the call (Yes/No)
Duration	Duration of the call in seconds or minutes
ProductSold	1 if a product was sold, 0 otherwise
Agent_Name	Name of the sales/call agent
🎯 Key KPIs Created
KPI	Description	Formula
Total Calls	Total number of calls made	COUNTROWS(dataset)
Calls Picked Up	Number of calls answered by customers	COUNTROWS(FILTER(dataset, PickedUp="Yes"))
Conversion Rate (%)	% of calls that resulted in a sale	(SUM(ProductSold) / COUNTROWS(dataset)) * 100
Average Call Duration	Average time per call	AVERAGE(Duration)
Total Products Sold	Total successful conversions	SUM(ProductSold)
📈 Visualizations Included

Cards — Display key metrics like total calls, sales, conversion rate.

Bar Chart — Show total calls and sales by each agent.

Pie/Donut Chart — Represent distribution of picked-up vs missed calls.

Line Chart — (Optional) Trend of calls or sales over time.

Slicers — Filters by Agent Name or PickedUp status for interactivity.

🎨 Dashboard Design Steps

Step 1: Import dataset into Power BI.
Step 2: Clean and format data using Power Query.
Step 3: Create DAX measures for KPIs.
Step 4: Add visualizations and arrange them in logical layout.
Step 5: Add slicers (Agent, PickedUp).
Step 6: Apply consistent color theme for clarity.
Step 7: Add navigation buttons and page titles.
Step 8: Export and summarize in PowerPoint presentation.

🧠 Insights

Agents with higher call pickups show higher conversion rates.

Shorter call durations often correlate with missed opportunities.

Conversion performance varies significantly among agents.
