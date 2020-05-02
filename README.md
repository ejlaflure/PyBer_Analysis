# PyBer Analysis
Analyze and visualize ride-sharing data using the capabilities of Python, Pandas and Matplotlib within Jupyter Notebook.

## Module Project Overview
Steps and Deliverables:
- Import your data into a Pandas DataFrame.
- Merge your DataFrames.
- Create a bubble chart that showcases the average fare versus the total number of rides with bubble size based on the total number of drivers for three city types.
- Determine the mean, median, and mode for the following:
  - The total number of rides for each city type.
  - The average fares for each city type.
  - The total number of drivers for each city type.
- Create box-and-whisker plots that visualize each of the following to determine if there are any outliers:
  - The number of rides for each city type.
  - The fares for each city type.
  - The number of drivers for each city type.
- Create a pie chart that visualizes each of the following data for each city type:
  - The percent of total fares.
  - The percent of total rides.
  - The percent of total drivers.

## Module Project Summary
Data Visualizations for PyBer Project:

![Fig1](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig1.png)
![Fig2](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig2.png)
![Fig3](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig3.png)
![Fig4](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig4.png)
![Fig5](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig5.png)
![Fig6](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig6.png)
![Fig7](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig7.png)

## Challenge Overview
This new assignment for you and Omar consists of three parts: two additional technical analyses and a written report that delivers your results to the CEO. To summarize, you will submit the following deliverables:
- Technical Analysis Deliverable 1: A DataFrame that summarizes the key metrics for the ride-sharing data by 
- Technical Analysis Deliverable 2: A multiple-line chart, with one line for each city type, that shows the sum of the fares for each week.
- Delivering Results: A written report of your results, saved in a README.md document on your GitHub repository.

# PyBer Analysis Report

## Background and Results

### Purpose
Analyzing PyBer's vast collection of data, will help us improve access and determine the affordability of our rideshare services in underserved neighborhoods. This is necessary for identifying valuable investment opportunities for our company moving forward. 

### Technical Analysis
To perform this task, I utilized the capabilities of Python, Pandas and Matplotlib. This enabled efficient analysis of PyBer’s raw data by quickly sorting and comparing multiple variables and creating visualizations to outline the treads of our company’s performance and operations. Below are examples of the code necessary to meaningfully compare the data and create visualizations.

![assemble_dataframe](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/assemble_dataframe.PNG)
![linegraph_creation](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/linegraph_creation.PNG)

### Results

![Table1](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Table1.png)
![Fig8](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig8.png)

### Summary
The table above shows a problematic trend that needs to be addessed. In urban cities, there are too many drivers for the avaliable riders in that area. To increase revenue along with rider and driver statisfaction, urban drivers should be adivised to operate in suburban and rural areas nearby. This will better distribute the drivers according to demand. 

The graph above shows that the end of Febuary is a times where more revenue is generated in all areas. Suburban and rurel areas are more consistent in March while urban areas are much more volitle.  During the end of March and beginning of April, some suburban drivers sould operate in rurel areas nearby to help accomidate the higher demand. 

## Challenges Encountered and Overcome

### Challenges and Difficulties Encountered

* Programming

While sorting the data to create the Total Fare by City Type graph, I ran into an issue with the resample method. This method sorts datetime data into bins based the chosen date or time type. For a graph encompassing four months, converting the data to weekly bins was necessary to have proper amount of data points for the graph. During this programing process, the resample method was not operating as I expected it would. 

* Data Analysis

After creating a new summary DataFrame that would show total riders, driver and fares along with average fare per diver and rider for each type of city, I wanted to represent this data in a table for quick and convenient analysis. I could have taken a screenshot of the table generated by Jupyter Notebook, but I wanted the code to automatically save the table as a picture. 

### Technical Analyses Used

* Programming

To overcome the programing issue, I researched and discussed the issue with my colleagues. Through this, I found that the issue was my index was not set to the data type datetime, which is necessary for the resample method to operate properly. Below is the code I created to rectify this problem. 

![datetime_index](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/datetime_index.PNG)

* Data Analysis

I researched panda's matplotlib's table creation capabilities and found that a table can be created and saved with matplotlib very similarly to how plots are generated from DataFrames. Below is the code I created to generate the table used in the PyBer Analysis Results. 

![table_creation](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/table_creation.PNG)

## Recommendations and Next Steps

### Recommendations for Future Analysis

Further analysis needs to be performed to more thoroughly identify issues in meeting ride demand.  This analysis is important for better utilizing divers and increasing revenue. 

### Additional Analysis 1

* Description of Approach

The first additional analysis that should be performed to meet this goal is a visualization comparing total fares over time to total rides and total drivers plotted over the same time period. This will complement that graph and will allow us to determine if the change in revenue at different periods is based on increased fare at that time or increased business.

* Technical Steps

To create this graph, a pivot chart will then need to be created along with new weekly bins, just like when created the Total Fare by City Type graph for number of rides and number of drivers. The creation of the graph at that point will also be the same as the Total Fare by City Type, but created for total rides and total drivers instead. Below is the code necessary to accomplish this task along with the results.

![table_creation](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/additional_analysis1.PNG)

* Results

![Fig9](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig9.png)
![Fig10](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig10.png)
![Fig11](https://github.com/ejlaflure/PyBer_Analysis/blob/master/Analysis/Fig11.png)

Total fares and rides show a direct correlation confirming that the increased revenue is from increased usage, but the total drivers are far more sporadic and to not directly relate. This shows that the amount of drivers is not related to demand in the area.

### Additional Analysis 2

* Description of Approach

The second additional analysis that needs to be performed is an overlay of average riders, drivers and fares per city. This is an analysis necessary to establish if there are particular cities that have a history of high demand or low demand vs sufficient drivers.

* Technical Steps

To create this new plot, the groupby function will be used to sort data based on cities. We will then use a multi-layered bar chart for visualization of this analysis. Below is the code necessary to accomplish this task along with the results.



* Results




