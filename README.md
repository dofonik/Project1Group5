# Project1Group5

Project Title: Australian Vehicle Trends

Team Members: Dominik Foale, Anrie Santos, Husna Nasution

Project Outline: Looking at recent vehicle listing data in Australia, we aim to perform exploratory data analysis to determine relationships between different variables and find trends in vehicle sales.

Research Questions to Answer:
1. How does car price vary by location and location average income?
2. How much does engine size (engine volume and number of cylinders) affect fuel consumptions?
3. What are the dominant vehicle brands and types in the Australian market?

Datasets to be used:
Australian Vehicle Prices​ - https://www.kaggle.com/datasets/nelgiriyewithana/australian-vehicle-prices/code
Average weekly ordinary time earnings, full-time adults by state, original​ - Australian Bureau of Statistics data
Australia Geo Postcode​ - https://gist.github.com/randomecho/5020859

Rough Task Breakdown:
Anrie - Q1

Husna - Q3

Dom - Q2
    Extract float/int values of fuel consumption, engine volume and cylinder count.​
    Clean the data of any NaN or 0 rows for these data columns.​
    Create box plot analysis of fuel consumption per number of cylinders in engine.​
    Perform linear regression comparing engine volume to fuel consumption.​

Github Description:
Inside of the AU Vehicle Prices Analysis are four folders (Q1, Q1, Q3 and raw_data). The raw_data folder contains CSV files of the original datasets analysed to answer the project questions. The Q1, Q2, Q3 folders contain ipython notebook files of the main code used to analyse the data for each question respectively. There are also image files of the plots that the main codes produce in each folder as well. Each notebook file can be run independently.

Summary of findings:
Q1

Q2 - How much does engine size (engine volume and number of cylinders) affect fuel consumptions?
![Alt text](FuelConsumption_BoxPlot.png)
![Alt text](FuelConsumption_linear_regression.png)

The box plot analysis comparing number of cylinders to fuel consumption indicates that, as a trend, fuel consumption increases with more cylinders. The median fuel consumption of vehicles with 2 engine cylinders is 4.2L/100km which is the lowest median fuel consumption. The median increases up to 7.3L/100km and 8.9L/100km for 4 and 5 engine cylinder vehicles respectively, and it increases to 16.5L/100km for the most cylinders considered which is 12.

The linear regression analysis revealed a significant positive correlation between engine volume and fuel consumption. The regression model equation was y = 1.73x + 3.70, suggesting that every extra litre of engine volume increases fuel consumption by approx. 1.73L/100km. The R-value of 0.746 indicates that this is a strong positive correlation. The standard error for this linear regression was 0.017, this low value suggests that our data set values are closely modeled by our linear regression.

Our analysis suggests that consumers that prioritise fuel efficiency should opt for vehicles with smaller engine volumes and cylinder counts. Similarly for manufacturers, the relationship found between fuel consumption and engine size (cylinder count and total volume) should be considered to properly engineer a vehicle for its target consumers (that being fuel economy focused consumers or power oriented consumers).

Conclusion - From our analysis, engine volume is directly associated with higher levels of fuel consumption with an average increase 1.73L/100km per 1 litre increase in engine volume. The number of cylinders present in a vehicle engine is also correlated to increased fuel consumption, as the median fuel consumption of the engine increases steadily as cylinder count is increased.

Q3

References:
Boxplot median extraction method created with help from:
https://matplotlib.org/stable/gallery/statistics/boxplot_demo.html