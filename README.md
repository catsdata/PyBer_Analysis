# PyBer Analysis

<details><summary>Table of Contents</summary>
<p>

1. [Overview](https://github.com/catsdata/PyBer_Analysis#overview)
2. [Resources](https://github.com/catsdata/PyBer_Analysis#resources)
3. [Results](https://github.com/catsdata/PyBer_Analysis#results)
    - [Total Rides](https://github.com/catsdata/PyBer_Analysis#total-rides)
    - [Total Drivers](https://github.com/catsdata/PyBer_Analysis#total-drivers)
    - [Total Fare](https://github.com/catsdata/PyBer_Analysis#total-fare)
    - [Average Fare per Ride](https://github.com/catsdata/PyBer_Analysis#average-fare-per-ride)
    - [Average Fare per Driver](https://github.com/catsdata/PyBer_Analysis#average-fare-per-driver)
    - [Weekly Fares Line Chart](https://github.com/catsdata/PyBer_Analysis#weekly-totals-by-city-type) 
4. [Summary](https://github.com/catsdata/PyBer_Analysis#summary)

</p>
</details>

## Overview

Explain the purpose of the new analysis.

## Resources

- Data Sources: [city_data.csv](https://github.com/catsdata/PyBer_Analysis/blob/main/Resources/city_data.csv) & [ride_data.csv](https://github.com/catsdata/PyBer_Analysis/blob/main/Resources/ride_data.csv)
- Software: 
    - Jupyter Notebook 6.4.6
    - Python 3.7.11 with dependencies: 
        - Pandas 1.3.5
        - MatPlotLib 3.5.0
    - Anaconda Command line Client 1.9.0
    - Conda 4.11.0


## Results

The following dataframe shows the calculated counts, sums and averages based on city type.

![dataframe](https://github.com/catsdata/PyBer_Analysis/blob/main/analysis/pyber_summary_dataframe.png)

- ### Total Rides:
    With Total Rides, we see a significantly larger demand (68%) in Urban cities than Rural and Suburban.  This could be expected based on normal population levels and business activity within the City Types.
- ### Total Drivers
    Just as with Total Rides, the larger skew is towards Urban ride sharing.  However, the number of Urban Drivers to Rides is unbalanced with a surplus of at least 780 drivers not providing rides.
- ### Total Fare
    Urban Fares bring in 63% of the toal 4 month revenue of $63,538.64, Suburban 30% and Urban only 7%.
- ### Average Fare per Ride
    Despite fewer rides and drivers, Rural brings in the highest average fare per ride, followed by Suburban.  This is opposite trending than the ride and driver counts, indicating a higher fare the further out from the city you go.
- ### Average Fare per Driver
    Just as the average fare per ride, Rural takes a substantial lead in average fare by driver.  The Urban averages are skewed by the unbalanced supply and demand of drivers to rides respectively.

- ### Weekly Totals by City Type
    The below multiple line plot of the three city types' weekly fare totals can assist in showing trending.  Just as we saw with the counts overall, Urban maintains the highest revenue each week, followed by Suburban and then Urban.  However, spikes and drops have consistency over all three city types between the end of Feburary and mid-March.  
  
![pyber_fare_summary.png](https://github.com/catsdata/PyBer_Analysis/blob/main/analysis/pyber_fare_summary.png)



## Summary

The following are business recommendations for the CEO addressing disparities among the city types:

1. There is a heavy saturation of drivers in Urban areas, with over 780 drivers not picking up rides.  There is more of a demand vs supply in the Suburban and Rural areas that could possibly benefit from the assitance of more drivers.  Perhaps work with Urban drivers, educating them about the higher per ride rate that could benefit them for going out of their normal area.   In addtion, consider evaluating the drivers employed.  Are they always available?  Part time?  Are there drivers that have stopped taking rides or have never taken any?  There may be a skew of counts on active vs inactive, or even seasonal, drivers.  If this information is already available, consider rerunning this data with the additional "available drivers" condition.  

2. The spikes and drops in rides over all three city types from the end of Freburary to the middle of March needs some futher evaluation.  These are time frames that perhaps can be monopolized upon.  Events, holidays, weather patterns and more should be considered.  Knowing these ups and downs can help control the driver to ride ratios during peek times.

3. There is a substantial profit level in the Rural and Suburban markets, however rides and drivers are low.  This could be an area where additional marketing to riders can benefit.  Perhaps there's not enough advertising getting to those populations.  On the flip side, the Urban market has a much lower average fare rate, which could indicate mostly short trips.  Consider a base or minimum cost despite mileage over all markets.

