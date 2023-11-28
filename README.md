# MSBA-Capstone-Maverik - Rachel Butterfield

### Project Goal: 

Maverik will be able to implement the model created to predict daily sales for diesel fuel, unleaded fuel, merchandise, and food sales for the entire first year of a store's operation. This model needs to surpass the accuracy metrics used by the current Maverik model in predicting these 4 product sales.

### Business Problem: 

Maverik, a convenience store and gas station chain with 300+ locations in the Western United States, aims to enhance its ability to assess the return on investment (ROI) for new stores, which are opened at an average rate of 30 per year. To achieve this, they require a new model capable of generating daily sales projections for merchandise, food sales, and total gallons sold for diesel and unleaded fuel for the entire first year of a store's operation.

This data-driven approach will enable Maverik to closely monitor the performance of new stores, make informed decisions, and promptly address any underperforming outlets. Maverik desires to know the daily sales for each of the 4 main products diesel fuel, unleaded fuel, merchandise, and food sales. Having these daily predictions allows for better planning for seasonality and setting realistic goals and expectations for what each new store can bring in revenue for the year.

### Analytic Problem: 

The target variables are daily sales for diesel, unleaded fuel, merchandise, and food services. Represented in the time_series_data_msba.csv sets of time series sales data where the variables.
daily_yoy_ndt.total_inside_sales: Inside sales, everything that isn't made at the store
daily_yoy_ndt.total_food_service: Food service sales, everything that is made at the store
diesel: Diesel gallons sold
unleaded: all non-diesel gallons
The main level of accuracy that we will use to determine the performance of this model is RMSE. 

Predict the daily sales for each 4 products diesel, unleaded fuel, merchandise, and food service for each store for the following year based on the time series data.

The success of this project will be measured by its capacity to accurately predict sales metrics and its usability for future stores. Our team will be judging our model based on RSME results. Since our target variables are numeric, we will explore which data features are significant via a linear regression model and then apply those features to a variety of data modeling techniques including a time series model.

### Solution to the Business Problem:

My group built a variety of models including Linear Regression, ARIMA, SARIMA, Exponential Smoothing, XGBoost, Neural Network and Prophet to see if we could produce a model that performs better than the Naive model that Maverik is using. We settled on the Prophet model as our final model to present to Maverik, as it resulted in the lowest error metrics. In training it performed up to 26% better than a general Naive model and up to 17% better when testing for certain stores. It was also able to predict target variables as close to 12% of the actual sales figures. The RMSE values it produced when compared to Maverik's model was significantly lower. 

### The Business Value of the Solution:

We broke the business value this model would add into four different categories including marketing, finance, operations, and management. This model would provide insight to where and how sales could increase for marketing purposes. It shows which stores have the highest revenue growth opportunities. Operationally, Maverik would be able to anticipate the supplies needed to match the demand for each stores. From a management standpoint, Maverik would be able to anticipate earnings from stores to inform stakeholders. 

### My Individual Contribution: 

I built the linear models to see if any of the variables in the dataset were significant and then applied that information as much as possible to my four Prophet models. The Prophet models aggregate the entire combined datasets while capturing daily, yearly, and holiday seasonality. Each Prophet model then predicts future sales for a single target variable for a single store. Tuning the models and testing each store on each model was a time intensive activity. I also compiled the three separate notebooks into this single group notebook for the group modeling assignment.

### Difficulties That My Group Encountered Along the Way:

My group worked extremely well together and didn't really run into any major problems. One small difficulty we found was trying to figure out how all our models worked and how to compare them to one another. Since Maverik had specifically said that RMSE should be used, we focused on that but also added some other error metrics as well. Another issue that popped up was that some of our models took a lot of computing power to run and we ended up adjusting the hyperparameters for them to run on our local machines. Ideally, we would have liked to further refine our model by grouping the dataset into clusters or build a ensemble model that combined our top performing models but were unable to due to time restraints. 

### What I Learned in the Project:

I learned a considerable amount working on this project. Time series modeling is something I had briefly touched on during my graduate program. Taking a real-life dataset and predicting sales for Maverik while trying to factor in multiple seasonality factors was challenging. To get the model to its final result took constant adjustment. The result of building a model that is an improvement on their existing model was very rewarding.

