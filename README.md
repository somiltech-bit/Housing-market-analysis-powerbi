# Housing-market-analysis-powerbi# Housing Market Analysis Dashboard

## Project Overview
This project is a Power BI dashboard built on a housing dataset of 100,000 rows to analyze house prices, sales trends, regional performance, and property characteristics. The dashboard was designed to help understand how purchase price, offer price, house type, region, and time-based factors influence the housing market.

## Objectives
- Analyze housing sales performance over time
- Compare offer price vs purchase price
- Study price trends across regions and house types
- Track YOY sales growth
- Identify factors influencing purchase price
- Analyze SQM price, inflation, interest rate, and bond yield patterns

## Dataset
The dataset includes:
- date
- quarter
- house_id
- house_type
- sales_type
- year_build
- purchase_price
- % change between offer and purchase
- no_rooms
- sqm
- sqm_price
- address
- zip_code
- city
- area
- region
- nominal interest rate %
- annual inflation rate %
- yield on mortgage credit bonds %

## Dashboard Pages
### 1. House Market Overview
Includes:
- Median sales price change by region
- Units sold in latest year and quarter
- Offer price vs purchase price
- YOY sales growth by sales type

### 2. Sales Performance
Includes:
- Sales by region
- Key influencers for purchase price
- Offer to SQM ratio by sales type
- Average price per SQM by region
- YTD sales tracking table

### 3. House Type Analysis
Includes:
- Avg offer price vs purchase price by house type
- Avg inflation, interest rate, and yield by house type
- Avg SQM and SQM price by house type
- Filters for area, city, sales type, and region

## Tools Used
- Power BI
- DAX
- Data modeling
- Data visualization

## Key Insights
- Regional sales and price patterns differ significantly across Denmark
- Offer price and purchase price are closely related, but vary by house type and region
- YOY growth varies by sales type
- SQM price and average property size show strong differences across house categories
- Macro factors like inflation, interest rate, and yield can be compared by house type

## Files in This Repository
- `powerbi/dashboard.md`
- `docs/data_dictionary.md`
- `docs/dax_measures.md`
- `docs/insights.md`
- `assets/page1.png`
- `assets/page2.png`
- `assets/page3.png`

## How to Use
1. Open the `.pbix` file in Power BI Desktop.
2. Refresh the dataset if needed.
3. Review the dashboard pages and filters.
4. Use the screenshots in `/assets` for quick preview.

## Author
Soumil Verma
