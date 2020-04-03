# Quality of Life in Austin, Texas
## Background
According to US News, Austin, Texas is declared to be the #1 city in America to live in because of its quality of life for the third time in a row. 

Although no correct system of metrics have been discovered yet to accurately measure quality of life, potential indicators that are important to a community are environmental qualities, nutrition/health, economic conditions/finances, security, education, and recreation. 
This cluster analysis explores different factors that may contribute to this ranking and groups different census tracts in Austin with Household Income, Incarceration Rates, Job Growth Rate, and Employment Rate as the metrics to analyze which parts of this big city is more attractive to live in as these factors have the most data and can be used to assess economic conditions, finances, and security. 
## Data Analysis
The cluster analysis has 3 clusters as it allows each group to embody distinctive qualities. The anchor tracts that resulted are **Springbrook, Pflugerville, TX** (cluster 1), **Austin, TX** (cluster 2), and **North Lamar, Austin, TX** (cluster 3). 

Cluster 1 (Springbrook)
1. Average household income
2. High job growth
3. Below average incarceration rates
4. High employment rate

Cluster 2 (Austin)
1. Very high household income
2. Very high job growth rate
3. Very low incarceration rates
4. Highest employment rate

Cluster 3 (North Lamar)
1. Below average household income
2. Low job growth rate
3. High incarceration rate
4. Low employment rate





### Additional Links and Sources
https://www.opportunityatlas.org
https://realestate.usnews.com/places/rankings/best-places-to-live

### Excel Steps
1. Export Opportunity Atlas Data on Household Income, Job Growth Rate, Incarceration Rate, and Employment Rate. 
2. Use VLOOKUP to have all the Data on one spreedsheet, and use paste special (values only) to insert into another spreedsheet for the cluster analysis. 
3. Calculate the mean and standard deviation for all 4 factors.
4. Use =STANDARDIZE to calculate the z-scores of every data point in each of the column factors. 
5. Name 3 arbitrary trial values for the 3 anchor points and use VLOOKUP to lay out their names and z-scores in an above chart. 
6. Use SUMXMY2 to figure out the 3 distances from each data point in each variable to the assigned trial values' z-scores. 
7. In another column, find the minimum value in the 3 distances using MIN formula. In an above cell, find the sum of the minimum distances.
8. Use MATCH to figure out which column the minimum distance belonged to and assign a cluster number to each row. 
9. Use the Solver tool. Cell is the sum of minimum distance cell, set to min, enter constraints (trial values cells >= 1, trial values cells are an integer, trial value cells <=265), set to evolutionary
10. The more accurate anchor points will result. Use conditional formatting to color code each cluster for better display. 
11. Determine the characteristics of each cluster. 

Define an initial business question
Define the data-related questions and metrics
Perform calculations and model-building to answer the data-related questions
Relate the data findings back to your initial question and outline what your cluster model tells us about the related organization
A brief description of your findings and background data with at least one data visualization
An outline of your business question → data question → data answer → business answer process and findings
