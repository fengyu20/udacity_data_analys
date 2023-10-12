# Udacity Data Analyst Nanodegree Projects (2020)

Welcome to my repository of projects completed in 2020 as part of the Udacity Data Analyst Nanodegree. I'm delighted to showcase my work and the valuable experiences and insights that I've gained throughout the course.

## Language Note
Please be informed that the original work and code documentation in this repository are primarily presented in Chinese. However, I have provided detailed explanations and overviews in English for each project.

## Project Introductions
### Flight Delay Forecast
Analysed a 7.5 million row flight takeoff and landing data set and made flight delay predictions using supervised learning algorithms, including Logistic Regression and GBDT.

### Bike-sharing Dataset Exploration
Conducted multi-variable analysis and created visualisations using Seaborn.

#### Dataset Introduction
The Mobike dataset contains approximately 102,361 cycling data entries, including Order ID (orderid), Bicycle ID (bikeid), User ID (userid), Start Time of Riding (start_time), Start Location (start_location_x, start_location_y), End Time of Riding (end_time), End Location (end_location_x, end_location_y), and Riding Trajectory (track), among other attributes.

New columns such as whether it is a weekday (weekday), riding time (cycle_time), and riding distance (cycle_distance) were added based on the original information in the dataset. 1027 outliers were removed based on the 99th percentile of riding time (cycle_time); 1014 outliers were removed based on the 99th percentile of riding distance (cycle_distance).

####  Summary of Findings
In the "Exploratory Analysis of Mobike Dataset":
1. The univariate section explored the overall distribution of the start times of rides.
2. In the bivariate exploration:
   1. A new column, weekday, was introduced to differentiate between weekdays and weekends, creating a comparison of the distribution of start times on weekdays and weekends (distplot).
   2. By calculating the start and end times, a new column, time, was introduced to record riding duration, and outliers in riding times were removed using the 99th percentile, creating a distribution chart of start times and riding durations (pointplot).
   3. A distribution comparison chart (violin) of riding durations on weekdays and weekends was created.
   4. The distribution charts of start and end locations were observed, with outliers removed using the 99th percentile. No clear relationship was found in the scatterplot of riding duration against start and end locations.
   5. Based on the start and end locations, a new column, distance, was introduced to record riding distances, creating a regression relationship chart of riding distances and times (regplot).
3. In the multivariate exploration: The distinction between weekdays and weekends was applied to the distribution charts of start times and riding durations, and also to the regression relationship chart of riding distances and times.

####  Key Insights for Presentation
In the presentation, we will first introduce the comparative distribution charts of start times on weekdays and weekends, followed by the relationship of riding durations with start times and distances on weekdays and weekends.

1. **Distribution chart of start times on weekdays and weekends**: Different colors and legends will be used to intuitively show the impact of distinguishing between weekdays and weekends as a valid categorical variable on the dataset, applying to the operation of Mobike: how to plan bicycle scheduling during peak commuting times on weekdays in advance.
2. **Distribution chart of riding durations with start times on weekdays and weekends**: Different colors and symbols will be used to highlight the different characteristics of start times on weekdays and weekends, applying to the operation of Mobike: whether to offer customized riding packages that include longer riding durations specifically for weekend riders.
3. **Distribution chart of riding durations with distances on weekdays and weekends**: Different colors and symbols will be used to showcase the characteristics of riding distances on weekdays and weekends, applying to the operation of Mobike: whether to restore weekend riding scenarios, such as whether to ride and tour around popular scenic areas, as an entry point for operational activities.

- References: The function to calculate distance (distance) is referred from: https://kanoki.org/2019/12/27/how-to-calculate-distance-in-python-and-pandas-using-scipy-spatial-and-distance-functions/

Feel free to explore each project, and your feedback or inquiries are warmly welcomed!