![alt text](https://github.com/cosfer2804/Projects-Repository/blob/main/CitiBike/SS/Citi_Bike_logo.jpg) 

# FINAL PROJECT - EDA CITIBIKE BICYCLE SHARING

By: <br/>
[Thiago Costa](https://www.linkedin.com/in/cosfer-thiago/)<br/>

## Table of Contents
- [Scenario](#scenario)
- [Objective](#objective)
- [Data Set](#data-set)
- [Tools and Methods](#tools-and-methods)
- [Analysis](#models)
- [Insight](#insights)
- [Next Steps](#next-steps)

## Scenario
In this final project I studied the covid impact in CitiBike, a bicycle sharing in New York City. For these I did an exploratory analysis since the start of the operations (June 2013) until February 2022. Then I decided to compare March, April and May in 2019, 2020 and 2021 to see if had any changed in the customer behavior.

## Objective
* Check if covid had an impact in the customer behaviors while renting bicycles in New York City.

## Data Set
- Provided by CitiBike, see the info of the dataset [here](https://ride.citibikenyc.com/system-data);
-  Download the CitiBike [data](https://s3.amazonaws.com/tripdata/index.html);
- 104 excel files, one per month;
- Over 140 millions of rows;
- Two different data format - It was necessary to standardize them.

## Tools and methods

### Trello - using agile method (Kanban)
Trello is a visual work management tool. I used trello to organize and manage the activities, I divided the activities into four main groups: goal, to do, doing, done.

### Tableau
Tableau is a visual analytics engine that makes it easier to create interactive visual analytics in the form of dashboards. The main use of tableau was to visualize and deep dive in the data to find customer behaviour patterns. The data that I used in this study had more than the limit provided by tableau public, so if you want to see the dashboards you need to download it. Check my [dashboards](https://github.com/cosfer2804/ironhack_final_project/tree/main/Tableau).

### Python
I divided the work done in python into four notebooks.
In the [concat - newformat](https://github.com/cosfer2804/ironhack_final_project/blob/main/Python/concat%20-%20newformat.ipynb) I merged the months that had the new format in one csv excel file, from January 2021 until February 2022. I decided not to use 2022 in my EDA because I had only two months to work with.

In the [concat - newformat](https://github.com/cosfer2804/ironhack_final_project/blob/main/Python/concat%20-%20newformat.ipynb) I merged the months that had the old format in one csv excel file per year, from June 2013 until December 2020 - input 91 excel files, output 9 files.

In the [eda - new format](https://github.com/cosfer2804/ironhack_final_project/blob/main/Python/eda%20-%20new%20format.ipynb) and [eda - old format](https://github.com/cosfer2804/ironhack_final_project/blob/main/Python/eda%20-%20old%20format.ipynb) I standardized both formats in one to work with them together on Tableau.

### Analysis
#### Overall
First it was necessary to understand the overall. In the plot below we can see how the amount of trips worked over the years.

<img width="1000" alt="Overall" src="https://github.com/cosfer2804/Projects-Repository/blob/main/CitiBike/SS/overall.png">

In this plot we see that normally the renting drops during the winter (or cold weeks) and increase in summer or good weather days. Also, it’s possible to see that covid dropped the amount of the trips, specially in the first restrictions. Soon after, trips begin to increase again, but in 2020 the amount of trips decreased nearly 5% in comparison to 2019.

As we look at the "Trips by Day" chart, we see that in 2020 (with more strict restrictions for covid), for the first time trips on Sunday and Saturday were more popular than weekday trips.

If we look at the users type the number of trips for casual users increased in 2020 and 2021.

After these analyses, I decided to dig deep and try to understand the impacts of covid on the bike rental system. To do this, I analyzed the months of March, April and May 2019, 2020 and 2021. All the next installments are filtered with this time frame.

PS: The colors of the users type is going to be the same in 'the Average Trips Duration'. Dark blue for casual users and light blue for member users (those who annually pay for a membership)


#### Station Growth
In the gif below we see the growth in the number of bicycle stations over the years.

![Alt Text](https://github.com/cosfer2804/Projects-Repository/blob/main/CitiBike/SS/gif%20station%20growth.gif)

#### Average Trip Duration

<img width="1000" alt="KNeighbors" src="https://github.com/cosfer2804/Projects-Repository/blob/main/CitiBike/SS/average_trip.png">

We can see from the graph above that the average trip duration per day in 2020 has increased compared to 2019. Also, in 2021 the average trip duration fell compared to 2020, still slightly higher than 2019, but seems to be returning to the pre-pandemic level.

#### TOP 10 Stations 

The last step of this project was to analyze the top 10 stations in March, April and May 2019, 2020 and 2021 and see if they changed during the pandemic. The intensity of the colors is based on the amount of trips at these stations during this period.

<img width="1000" alt="KNeighbors" src="https://github.com/cosfer2804/Projects-Repository/blob/main/CitiBike/SS/TOP10%20stations.png">

As we can see above, the most popular stations in 2019 were nearby other public transportation stations. For example, Pershing Square North is nearby NYC Central Station.

When analyzing the most popular stations during weekdays, we can see that stations closer to tourist areas and recreational areas were the most popular in 2020. It's worth noting that they are similar to the popular stations in 2019 during weekends.

In 2021, stations that were popular in 2019 and stopped being in 2020 reappear. But in general, the most popular stations continue to be close to leisure and tourist areas.

### Insights
FALTA ATUALIZAR!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
* When we combine the insights from all the plots it's possible to see that
* People in 2020 were using CitiBike as leisure, instead of going to work. At the same time, we see that casual trips increased, maybe because people thought that wasn't worth to buy the subscription for all the year without knowing what was going to happen with covid.
* 2021 seems to start going back to normality, but still far from it.
* In 2020, even with the pandemic, the amount of trips dropped only 5%, but in 2021 increased 41%. 

### Next Steps
Check if in the future the customer behavior changed only during the pandemic or if covid created new pattern over the next years.
