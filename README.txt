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

1. Issue and recommendation:
we have order has a missing customer city we will validate the city field and correct or exclude the record from city-level reporting.
2. Issue and recommendation:
One order has a zero quantity and a duplicate order exclude orders with non-positive quantities and remove duplicate orders based on order_id before reporting.
## What the pipeline does
Complete after the lab: In one sentence, describe how the data moves from the source to a useful output.
