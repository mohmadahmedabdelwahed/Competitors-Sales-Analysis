# Competitors-Sales-Analysis
This project analyzes Sintec’s sales performance against major competitors across multiple countries using Power Query for data preparation and Power BI for reporting.

## Business Problem: 

Sintec wants to evaluate its competitive position in the market, not just internal performance. 

They need visibility on: 

1. How competitors perform across countries 
2. Which categories and segments drive the most revenue 
3. Growth opportunities 
4. Market share evolution over the years 
5. Top-performing products compared to competing offerings 

This project provides a complete analytics solution to guide strategic decisions.

## Summary:
This project analyses Sintec’s sales performance against four major competitors across multiple countries using Power Query for data preparation and Power BI for interactive reporting. 

I cleaned and transformed multiple datasets (Sintec + competitor sales (fact table), product, manufacturer table, and geography table (dimension tables)) by merging tables, transposing dimensions, filling missing values, and filtering the data to the last three years (2019–2021). 

The final Power BI report identifies market leaders, top-performing products, revenue trends, and Sintec’s market share evolution. 

## Key Findings:

1. Sintec leads revenue in the USA, outperforming its closest competitor (Ductal) by $7M. 
2. Sintec underperforms outside the USA — especially in Canda where competitors like Artisans reach $3M vs Sintec’s 956,405.36 thousand. 
3. Artisans is the global market leader, followed by Sintec, with a difference of $39M. 
4. Urban category generates 78% of total revenue across manufacturers. 
5. Youth segment shows the highest 3-year growth at 64.5%, for all companies and 86.81% for sintec. 
6. intec’s global market share is 19.7% over the three years. 
7. Market share increased 1% (2019→2020) and 1.45% (2020→2021). 
8. Key Influencers highlight that product “Sintec UC-19” increases revenue by +290.5, signalling a high-priority product.

![Image Alt](https://github.com/mohmadahmedabdelwahed/Competitors-Sales-Analysis/blob/d6739370ebcf241c216f9be325a74ec80d00b48c/1.%20Competitors%20Sales%20analysis.png)

![Image Alt](https://github.com/mohmadahmedabdelwahed/Competitors-Sales-Analysis/blob/d6739370ebcf241c216f9be325a74ec80d00b48c/2.Advanced%20Insights.png)


## Business Recommendations:

1. Invest more in Japan and other non-USA markets where Sintec’s share is significantly lower 
2. Focus on high-impact products such as Sintec UC-19 
3. Increase production and marketing in the Urban category, the largest revenue driver 
4. Allocate strategic resources to capitalize on Youth segment growth 
5. Benchmark heavily against Artisans, the dominant global competitor 
6. Maintain momentum as Sintec’s market share shows steady YoY increase 

## The entire dataset is organized in a snowflake schema with one fact table and multiple dimensions. 

![Image Alt](https://github.com/mohmadahmedabdelwahed/Competitors-Sales-Analysis/blob/d6739370ebcf241c216f9be325a74ec80d00b48c/3.data%20model.png)


## Methodology 

1. Data Modelling: Schema: Snowflake, Fact Table: Sales, Dimension Tables: Products, Manufacturers, Geography, and a Date table (DAX-generated) 
2. Data Loading: Loaded USA sales separately, Combined international sales (6 countries) into one unified table, Converted ZIP codes, standardized types, and added missing country data, Limited the fact table to 2019–2021, Data Cleaning & Transformation (Power Query), Removed redundant columns (e.g., Source), Filled missing product categories , Split Price column → Currency + Price ,cleaned geography table headers , Transposed manufacturer table ,Added a Country column to appended international sales, Created concatenated keys in Sales & Geography to build relationships, Disabled intermediate queries from loading.

3. Data Exploration (Power BI): 
Revenue analysis by manufacturer, country, and product hierarchy, Category & segment drilldowns, Year-over-year revenue comparisons using DAX, PY Sales (SamePeriodLastYear), Growth% measures 

4. Visualizations: 
Stacked column charts, Line charts, Decomposition tree, Key influencers, Clustered bar charts, Market share matrix 

5. Skills Demonstrated 
Power Query transformations, Data modelling (Snowflake schema), DAX calculations for YoY analysis, Complex relationships creation (concatenated geographic keys), Advanced visualizations (Key Influencers, Decomposition Tree), Market share analysis, Data storytelling, Business insight generation



