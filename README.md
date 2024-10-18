## Overview
This project conducts a comprehensive analysis of demand, operational costs, and capacity utilization for different transportation routes. It utilizes R programming, leveraging libraries like `dplyr` for data manipulation and `ggplot2` for visualization.

## Packages
The following R packages are required for this analysis:

```r
# Libraries
library(dplyr)      # For data manipulation
library(ggplot2)    # For data visualization
```

## Generating Data
This section generates synthetic data for demand forecasts and operational costs:

- **Demand Forecasts:** Randomly samples from defined routes and months to create a demand dataset with normally distributed demand values.
- **Operational Costs:** Generates random operational costs (fuel, labor, maintenance) for each route based on predefined means and standard deviations.
- **Route Capacities:** Defines static capacities for each route in terms of weight (tons) and volume (cubic meters).

The generated datasets include:
- `demand_data`: Demand forecasts per route and month.
- `operational_costs`: Costs associated with fuel, labor, and maintenance per route.
- `route_capacities`: Static data representing route capacities.

## Demand Analysis
This section analyzes demand trends across different routes:

1. **Demand Summary Statistics:** Calculates mean, median, standard deviation, and total demand for each route.
2. **Monthly Demand Trends:** Summarizes monthly demand for each route and visualizes trends using line plots.

Output:
- Summary statistics printed to the console.
- A line plot showing monthly demand trends for each route.

## Operational Cost Analysis
This part focuses on analyzing the total operational costs for each route:

1. **Total Cost Calculation:** Computes the total operational costs by summing fuel, labor, and maintenance costs.
2. **Cost Visualization:** Creates a bar chart to visualize total operational costs per route.

Output:
- Total operational costs printed to the console.
- A bar chart representing total costs for each route.

## Capacity Utilization Analysis
This section evaluates how well each route's capacity is utilized based on the demand data:

1. **Utilization Calculations:** Merges demand summaries with route capacities to calculate utilization rates in tons and volume.
2. **Utilization Visualization:** Visualizes the capacity utilization using a bar chart that compares utilization rates for weight and volume.

Output:
- Capacity utilization data printed to the console.
- A bar chart comparing capacity utilization (in tons and volume) for each route.

## Conclusion
This analysis provides valuable insights into demand patterns, operational costs, and capacity utilization, which can aid in strategic decision-making for transportation logistics.
