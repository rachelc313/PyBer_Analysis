# PyBer_Analysis
## Overview of the Analysis
Using two large CSV files of 2019 data provided by Pyber, a Python-based ridesharing app company, to find disparities and make recommondations to the CEO for addressing such disparities.

 1. How many city types were reviewed? Provide a breakdown of the total rides, total drivers, total fares, and their percentages. What were the average fare per ride for each city type? Per driver?
 2. Which city types had the highest total rides, total drivers, and total fares?
 3. Which city type had the lowest total rides, total drivers, and total fares?
 4. Which city type had the highest average fare per ride? Per driver?
 5. Which city type had the lowest average fare per ride? Per driver?


## Resources
 - Data Sources: city_data.csv, ride_data.csv
 - Software: Python 3.7.13

 ## Results
 
The analysis of the Pyber data provided show that:
  - Three city types were reviewed: "Rural", "Suburban", and "Urban".

    - "Rural":
        - Total rides: 5.3% (125)
        - Total drivers: 2.6% (78)
        - Total fares: 6.8% ($4,327.93)
        - Average fare per ride: $34.32
        - Average fare per driver: $55.49
    - "Suburban": 
        - Total rides: 26.3% (625)
        - Total drivers: 16.5% (490)
        - Total fares: 30.5% ($19,356.33)
        - Average fare per ride: $30.97
        - Average fare per driver: $39.50
    - "Urban": 
        - Total rides: 68.4% (1,625)
        - Total drivers: 80.9% (2,405)
        - Total fares: 62.7% ($39,854.39)
        - Average fare per ride: $24.53
        - Average fare per driver: $16.57
 - The "Urban" city type had the highest total rides, total drivers, and total fares. They had the lowest average fare per ride and driver compared to the other two city types.
 - The "Rural" city type had the lowest total rides, total drivers, and total fares. They had the highest average fare per ride and driver compared to the other two city types.
## Summary
Below are recommendations to address the disparities among the city types:
- The disparities are most likely explained by the distance of the rides themselves. Perhaps in rural cities, offering a larger payout to cover gas expenses but also increasing the price of the rides so there is incentive for the current drivers to drive more.
- Incentives could be offered to drivers from surrounding cities to go into the rural cities and take more rides. Perhaps Urban drivers could be offered such an incentive starting at the end of April when the fares drop significantly. Before making this decision, a closer look into what drops, when and why would be necessary.
- As seen in the below line graph: towards the end of February, each of the city types had a spike in fares. Taking advantage of this, and increasing at least the Rural and Suburban prices could be beneficial. 



## Limitations
Below are limitations in the provided dataset:
- After the two DataFrames were merged into a single dataset, there was a discrepancy found when calculating the driver counts using the merged dataset. Upon further investigation, there were 2255 "city" duplicates found. These rows could not be removed because the other columns are critical to the analysis. For this area, the "city_df" DataFrame was used to accurately count the number of drivers for each city type. 