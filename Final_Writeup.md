# Linear Regression of Movie Theater Gross with CDC Vaccination Data
Alex Stake

## Abstract

The goal of this project was to attempt to predict the domestic gross of movies using primarily release date features and how they interacted with vaccination data for Covid-19. This was attempted through a linear regression model, using regularization models such as LASSO to even out features and decrease overfitting. Despite the use of LASSO, the model is overfitting the data and further exploration of regression methods such as time series should be explored.

## Design

The goal was to initially demonstrate the recovery of the theater industry by showing the increasing growth of domestic box office gross by the increasing number of vaccinations as well as to include other factors into the gross. 

## Data

The primary data used was box office data from boxofficemojo that was scraped using BeautifulSoup covering the years 2020 and 2021. This data was then combined with CDC Covid-19 vaccination data that was freely available for downloading. Some features of the data included the daily gross, the number of theaters the movie was released in, the distributor of the movie, the number of fully vaccinated (1 or 2 shots) people, and the locations these people were vaccinated. 

## Algorithms

Linear regression was the primary model used, with feature engineering used for several categorical features. This model was then tested and found to have an R-squared value of 0.71039 and a Mean of Absolute errors(MAE) of 8,010,208.31, or ~$8 million. This model was cross validated and had regularization used in the form of LASSO and Ridge regression, but was still found to perform as well as either regularized model. The final R-squared value of the linear regression model was found to be 0.69188 with an MAE of 9606285.61, or ~$9.6 million.
## Tools

- BeautifulSoup for webscraping
- Pandas and Numpy for data exploration and cleaning
- Seaborn for visualization
- Scikitlearn for modeling

## Communication

The data is presented through the ![slides](https://github.com/ajstake/Linear_Regression_Project/blob/main/Theaters_in_Covid_presentation.pdf) provided.
