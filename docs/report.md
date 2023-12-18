# DATA606 - Capstone Project

**Project: Flight Price Prediction**

**Presentation Video: <https://www.youtube.com/watch?v=4q1UohPmPtg>**

**Project PPT:**

[**https://github.com/DATA-606-2023-FALL-TUESDAY/Meruva_LohithReddy/blob/main/docs/Capstone_Final.pptx**](https://github.com/DATA-606-2023-FALL-TUESDAY/Meruva_LohithReddy/blob/main/docs/Capstone_Final.pptx)

## 1.Introduction

In the dynamic and competitive world of air travel, understanding the
factors influencing airline ticket pricing is crucial for both consumers
and industry players. This report presents a comprehensive analysis
aimed at predicting airfare prices, leveraging data primarily sourced
from the \"Yatra\" website. Our investigation delves into various
aspects such as airline differences, class variations, and the impact of
timing on airfares. Employing advanced regression models and machine
learning techniques like XGBRegressor, we seek to unravel the
complexities of airfare pricing. This study not only offers valuable
insights into current pricing strategies but also serves as a predictive
tool for future fare trends, thereby aiding decision-making processes
for stakeholders in the airline industry.

## 2. Research Questions

i)  Do the timings of departure and arrival have an impact on the cost
    of a ticket?

ii) What is the impact of changing the source and destination on the
    price?

iii) What is the pricing difference between Business and Economy class
     tickets?

iv) Do prices change depending on the airline?

v)  When tickets are purchased only one or two days before to travel,
    how does the price change?

vi) Does the price vary depending on the number of stops?

vii) Which variables most affect the price?

## 3.Dataset Information

The dataset used for the flight price prediction project comprises
various attributes collected to understand and predict airfare trends.
It includes data on airlines, dates of journey, departure and arrival
times, source and destination airports, routes, flight duration, total
stops, and additional information pertinent to travelers. The dataset
contains flight details of around 10682 Flights on different routes. The
dataset has 11 features like Airlines, Duration, Route, Price, etc. This
rich dataset forms the backbone of the analysis and modeling, enabling
the application of machine-learning techniques to forecast flight prices
with accuracy.

## 4. Methodology

i)  Data Preprocessing
- The 'Date_of_Journey' is converted into separate day and month columns to better understand seasonal trends. The flight duration is split into hours and minutes for a more granular analysis. Airlines, source, and destination data are processed to create distinct categories, which helps in understanding the influence of these variables on ticket prices.

ii) Exploratory Data Analysis

> The EDA involves data loading, cleaning, and preprocessing steps, such
> as handling missing values and converting date and time formats. The
> analysis creates derived features from the dataset, which includes
> information like the airline, date of journey, source, destination,
> route, departure time, arrival time, duration, total stops, additional
> info, and price. Key aspects of the EDA include grouping data by
> airlines to observe price variations and examining the impact of
> weekends on prices. The report also investigates price variation
> throughout the day by categorizing flight departure times and
> analyzing their frequency. This comprehensive approach helps in
> understanding the factors influencing airline ticket prices, setting a
> foundation for further modeling and prediction tasks.
>
> ![A graph of different colored bars Description automatically
> generated with medium
> confidence](vertopal_0924b84490584848929f84d5bf04745c/media/image1.png){width="5.1957425634295715in"
> height="3.5902777777777777in"}
>
> **Fig 4.1**
>
> For most airlines, ticket prices are consistent across weekdays and
> weekends. However, there is a significant increase in price for the
> Jet Airways Business class on weekends. This suggests a demand-based
> pricing strategy, where prices for certain premium services are raised
> on weekends, possibly due to higher demand or reduced availability.
>
> ![A graph of a graph Description automatically generated with medium
> confidence](vertopal_0924b84490584848929f84d5bf04745c/media/image2.png){width="5.298611111111111in"
> height="2.8271784776902886in"}
>
> **Fig. 4.2**
>
> The bar chart illustrates the distribution of flight departures across
> different times of the day. The \'Early Morning\' period has the
> highest count of departures, suggesting it\'s a popular time for
> flights. The \'Evening\' and \'Morning\' slots also show a significant
> number of departures, indicating a preference for starting travel
> early in the day. The \'Afternoon\' sees a drop in departures, with
> \'Night\' and \'Late Night\' having the fewest flights, likely due to
> lower demand and operational constraints during late hours. This
> pattern could inform airline scheduling and fare strategies.
>
> ![A graph showing different colored dots Description automatically
> generated](vertopal_0924b84490584848929f84d5bf04745c/media/image3.png){width="5.492357830271216in"
> height="2.9305555555555554in"}
>
> **Fig 4.3**
>
> The scatter plot shows the relationship between the total duration of
> flights in minutes and their prices in INR, with different colors
> indicating the number of stops (0 to 4). Generally, longer flights
> appear to be more expensive, and flights with more stops tend to have
> higher prices. Notably, there\'s a cluster of non-stop flights (0
> stops) with shorter durations that are the least expensive. As the
> number of stops and duration increases, so does the variability in
> price, with some long-duration flights (especially those with 3 or 4
> stops) reaching the highest prices.
>
> ![A graph of a graph with text Description automatically generated
> with medium
> confidence](vertopal_0924b84490584848929f84d5bf04745c/media/image4.png){width="5.6094936570428695in"
> height="2.9930555555555554in"}
>
> **Fig 4.4**
>
> The boxplot graphically depicts the distribution of prices for
> different airlines and classes. Each box represents the interquartile
> range of prices for that category, with the horizontal line inside the
> box indicating the median price. The whiskers extend to the furthest
> points considered to be within the normal range, and outliers are
> represented as individual points. Jet Airways Business class shows a
> significantly higher price range and median compared to other
> categories. This visual suggests variability in pricing strategies
> among different airlines and classes, with business classes generally
> positioned at higher price points.
>
> ![A graph of blue rectangular shapes Description automatically
> generated with medium
> confidence](vertopal_0924b84490584848929f84d5bf04745c/media/image5.png){width="5.661554024496938in"
> height="3.0208333333333335in"}
>
> **Fig 4.5**
>
> January shows the highest mean price, suggesting it might be a peak
> travel period, possibly due to holidays or festivals. April has the
> lowest mean price, indicating a potential low season for travel. The
> mean prices for September, May, June, December, and March are
> relatively similar, suggesting consistent pricing across these months.
> This information can help in understanding seasonal pricing trends in
> the airline industry.

iii) Feature Engineering

> The prediction of flight prices is most significantly influenced by
> the destination and airline, with importance scores of 0.998 and
> 0.974, respectively. Source cities, duration, and timing of the flight
> also impact prices to a lesser degree, while the travel date and year
> offer minimal to negligible predictability.
>
> ![A screenshot of a computer Description automatically
> generated](vertopal_0924b84490584848929f84d5bf04745c/media/image6.png){width="2.3541666666666665in"
> height="1.9108661417322834in"}

iv) Model Selection & Training

> Linear Regression
>
> R\^2 score for train dataset = 0.5899
>
> Lasso Regression
>
> R\^2 score for train dataset = 0.5897
>
> Random Forest Regression
>
> R\^2 score for train dataset = 0.9547
>
> Random Forest Regressor gives a maximum R2 score of 95.45 and a
> maximum cross-validation score.

## 5. Limitations & Future Scope:

-   In this study we focus on flights on one year of data and more data
    can be incorporated in this project to extend it beyond the present
    investigation.

-   This project aimed to develop a machine learning model that could
    accurately predict the fare of the ticket of features available in
    the dataset.

-   The web application assists the passengers in ticket bookings.

-   There is potential for improving the model\'s accuracy by
    incorporating additional features, expanding to more locations, and
    gathering more data, among other possibilities.

-   Time series analysis can be performed over this model.

-   This project can result in saving money for inexperienced people by
    providing them the information related to trends in flight prices
    and also giving them a predicted value of the price which they use
    to decide whether to book a ticket now or later. On working with
    different models

## 6. Takeaway Points

i.  The model that gives the best result is the Random Forest Regressor
    with on the train dataset on R\^2 score equals to 0.9547.

ii. The longer the flight is the more expensive the tickets are until it
    reaches around 20 hours, then the prices tend to decrease.

iii. The \'Early Morning\' period has the highest count of departures,
     suggesting it\'s a popular time for flights. The \'Evening\' and
     \'Morning\' slots also show a significant number of departures,
     indicating a preference for starting travel early in the day.

iv. There is a big gap between flight tickets in business and economy.
    In average business tickets are 6.5 times more expensive than
    economy tickets.

v.  For most airlines, ticket prices are consistent across weekdays and
    weekends. However, there is a significant increase in price for the
    Jet Airways Business class on weekends.

vi. January shows the highest mean price, suggesting it might be a peak
    travel period, possibly due to holidays or festivals. April has the
    lowest mean price, indicating a potential low season for travel.

## 7. References

i.  Masoud Soroush 602 Notes

ii. V. Rao and J. Sachdev, \"A machine learning approach to classify
    news articles based on location\",

iii. V. Kumar and S. Minz, \"Poem classification using machine learning
     approach\", Proceedings of the Second International Conference on
     Soft Computing for Problem Solving (SocProS 2012

iv. B.Pang, L. Lee and S. Vaithyanathan, \"Thumbs up? Sentiment
    classification using machine learning techniques\" in Language
