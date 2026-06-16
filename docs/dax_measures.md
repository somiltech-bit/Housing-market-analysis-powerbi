# DAX Measures

The following DAX measures were created to generate KPIs and business insights.

## Age

Calculates property age.

```DAX
Age = ABS(YEAR(Housing[date]) - Housing[year_build])
```

## Offer Price

Calculates estimated offer price.

```DAX
Offer Price =
(100*Housing[purchase_price])/
(100-Housing[%_change_between_offer_and_purchase])
```

## Average Price SQM

Calculates average price per square meter.

```DAX
Average Price SQM =
AVERAGE(Housing[sqm_price])
```

## Last 12 Month Sales

Calculates rolling 12-month sales.

```DAX
Last 12 Month Sales =
CALCULATE(
SUM(Housing[purchase_price]),
DATESINPERIOD(
Housing[date],
MAX(Housing[date]),
-12,
MONTH
))
```

## Median Sales Price Change

Calculates year-over-year median price change.

## Offer to SQM Ratio

Calculates offer price per square meter.

```DAX
Offer to SQM Ratio =
DIVIDE(
SUM(Housing[Offer Price]),
SUM(Housing[sqm])
)
```

## Sales by Region

Calculates total sales by region.

```DAX
Sales by Region =
CALCULATE(
SUM(Housing[purchase_price]),
ALLEXCEPT(Housing,Housing[region])
)
```

## Total YTD Sales

Calculates year-to-date sales.

```DAX
TotalYTD Sales =
TOTALYTD(
SUM(Housing[purchase_price]),
Housing[date]
)
```

## Units Sold (Latest Year & Quarter)

Counts houses sold in the latest period.

```DAX
DISTINCTCOUNT(Housing[house_id])
```

## YOY Sales Growth

Calculates year-over-year sales growth percentage.

```DAX
(Current Year Sales - Previous Year Sales)
/ Previous Year Sales
```
