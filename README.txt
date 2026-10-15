# Week 1 Data Engineering Lab

## Scenario
A small online shop sends daily order data as a CSV file. A manager wants a reliable summary of valid orders by city.

## Pipeline plan
- Source: `orders.csv` (daily batch file)
- Raw destination: BigQuery table `de_intro.raw_orders`
- Curated output: query results after checking and filtering the data
- User of the output: shop manager

## Local data check
Before reporting, record at least two issues you found in the CSV and what you recommend doing with each.

1. Issue and recommendation: the first problem is the missing data in the example as the “customer_city” in the fourth order, that it should be filled by gaining the info, but ifit was deleted the report of valid orders will be inaccurate
2. Issue and recommendation: the second is the wrong values data, that the fifth order has a quantity of “0” which cant be a valid order, it can be deleted

## What the pipeline does
Complete after the lab: In one sentence, describe how the data moves from the source to a useful output.
