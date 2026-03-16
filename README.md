# Ontario-Hotel-Performance-Analysis
This is a comprehensive analysis of the Ontario hospitality market over the period from February 2023 to December 2025. The study evaluates key hotel performance indicators, including Occupancy Percentage, Average Daily Rate (ADR), and Revenue Per Available Room (RevPAR) across different regions and cities in Ontario. 

## Data Source
The dataset was obtained from the Ontario Open Data Portal.
However, the raw data was not structured in a ready-to-use table format, and the files were provided as separate monthly Excel sheets. This required extensive data preparation before analysis.

## Data Preparation & Transformation (Power Query)
• Combined multiple monthly Excel files into a single dataset
• Cleaned and transformed the raw files into structured tables
• Applied transformations in one query that automatically propagated to all monthly files
• Standardized columns and data formats
• Appended monthly datasets to create a complete time-series dataset
This process ensured a scalable and automated data preparation workflow.

## Data Modeling
After cleaning the data, I built a star schema data model:
• Created a Fact Table containing hotel performance metrics
• Built a Date Dimension Table to enable time intelligence analysis
• Established one-to-many relationships between fact and dimension tables
This structure improved query performance and analytical flexibility.

## Measures & Analytics
Using DAX, I created several analytical measures, including:
• Recalculated KPIs as dynamic measures
• Month-over-Month (MoM) performance metrics
• Conditional formatting for KPIs (e.g., green for growth, red for decline)
• Time-based trend analysis using the date dimension

## Dashboard Development
The final Power BI dashboard includes multiple interactive visualizations:
• KPI Cards (Occupancy, ADR, RevPAR)
• Trend Analysis Charts
• Scatter Plot (ADR vs Occupancy relationship)
• Regional Performance Comparisons
• Geographic Map Visualization
• Top/Bottom Market Analysis
To enhance usability, I implemented:
• Bookmarks to switch between Province, Region, and City-level views
• Interactive slicers
• Dynamic MoM indicators with color-based insights

## Key Insights
• RevPAR increased from $139.64 (2023) to $142.09 (2025)
• The market shows strong seasonality, with peak demand in summer months
• Greater Toronto Area dominates hotel revenue performance
• North Western Ontario shows emerging growth potential
• Strong correlation between Occupancy and ADR, indicating effective dynamic pricing strategies in high-demand periods
