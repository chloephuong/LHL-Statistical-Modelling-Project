# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
Project Goal: Analyzing the Relationship between Bike Stations and Restaurants

The goal of this project is to analyze the relationship between bike stations and nearby restaurants in a chosen area. The project involves collecting data from multiple sources, including bike station data, and leveraging the Foursquare and Yelp APIs to gather information about nearby restaurants. The collected data will be combined and analyzed to gain insights into the interaction between bike availability and the restaurant landscape in the area.

## Process

1. Collect Data:

Obtain data on bike stations including their location (latitude and longitude) and the number of available bikes. This data is stored in the bike_df dataframe.

2. Gather Additional Data:

Utilize the Foursquare and Yelp APIs to retrieve data on nearby restaurants based on the bike station locations. Extract relevant information such as restaurant names, ratings, and location details.

3. Data Integration and Joining:

Combine the bike station data from bike_df with the restaurant data obtained from Foursquare and Yelp. Use a common key (e.g., latitude and longitude) to join the datasets, creating a comprehensive dataframe that includes bike station details and restaurant information.

4. Exploratory Data Analysis (EDA):

Perform EDA on the joined dataframe to gain insights into the relationship between bike stations and restaurants. Analyze factors such as the number of bikes, restaurant count, average ratings, and their distributions. Visualize the data through plots, histograms, or maps to identify patterns and trends.

5. Regression Model Building:

- Build a regression model using the Python statsmodels module to explore the relationship between the number of bikes and the number of restaurants and their average ratings. Use the joined dataframe as the basis for the model.
- Specify the dependent variable (number of bikes) and the independent variables (restaurant count and average rating).
- Train the regression model using the dataset and evaluate its performance metrics such as R-squared, F-statistic, and p-values.
- Interpret the results to understand the impact of restaurant count and average rating on the number of bikes at each station.

6. Interpret and Conclude:

- Interpret the findings from the regression and classification models to understand the relationship between bike stations and restaurants.
- Draw conclusions on whether the number of restaurants and their average ratings have an impact on the availability of bikes at each station.
- Summarize the insights and recommendations based on the analysis for stakeholders or further research.

## Results

Summary Result: Comparing API Coverage
- During the project, I compared the coverage and usefulness of two popular APIs, Foursquare and Yelp, for obtaining data on nearby restaurants. I found that the Yelp API provided more comprehensive and valuable information compared to the Foursquare API. Yelp offered additional details such as restaurant ratings, reviews, phone numbers, and images, which enriched the dataset and provided more insights into the restaurant landscape in the chosen area. Therefore, I concluded that the Yelp API was more helpful in this context.

Model Outcome: Relationship between Bikes, Restaurants, and Ratings
- Our regression model aimed to explore the relationship between the number of bikes at each station and the restaurant count, as well as the average rating of nearby restaurants. The model's results indicated a weak relationship between these variables. Furthermore, the p-values for the coefficients were not statistically significant, indicating that these predictors did not have a substantial impact on bike availability. In summary, the model did not find a strong relationship between the number of bikes and the restaurant count or average rating. 

## Challenges 

During the project, several challenges were encountered:

1. API Limitations: One of the main challenges was working with API limitations, including rate limits and access restrictions. Both the Foursquare and Yelp APIs had limitations on the number of requests that could be made within a specific timeframe. This required careful management of API calls and handling potential errors or restrictions.

2. Data Consistency: Integrating data from multiple sources (bike data, Foursquare, Yelp) posed challenges in terms of data consistency. Each API had its own data structure, naming conventions, and missing data. Ensuring proper data alignment and handling missing or inconsistent data required thorough data cleaning and preprocessing.

3. Joining and Merging Data: Joining and merging data from different sources can be complex, especially when there is no common key or when the data formats are different. Identifying appropriate keys and ensuring accurate merging required careful consideration and validation to create a unified dataset.

4. Model Interpretation: Interpreting the results of the regression model can be challenging, particularly when the model's performance is low or the predictors do not exhibit strong relationships with the target variable. It requires careful analysis and understanding of the model's limitations and potential confounding factors that may influence the results.

## Future Goals

If I had more time, there are several areas I would focus on to further enhance the project:

1. Expand Data Collection: I would explore additional data sources beyond Foursquare and Yelp to gather more comprehensive information about the bike stations and surrounding areas. This could include data on demographics, local events, transportation infrastructure, or weather conditions. By incorporating a wider range of data, the analysis would provide a more holistic understanding of the factors influencing bike usage and restaurant presence.

2. Feature Engineering: I would invest more time in feature engineering, exploring different combinations of variables and creating new features that capture meaningful relationships between the predictors and the target variable.