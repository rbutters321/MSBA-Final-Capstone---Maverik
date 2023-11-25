# MSBA-Final-Capstone-Maverik - Rachel Butterfield

### Project Goal: 

Maverik will be able to implement the model created in order to predict daily sales for diesel fuel, unleaded fuel, merchandise, and food sales for the entire first year of a store's operation. This model needs to surpass the accuracy metrics used by the current Maverik model in predicting these 4 product sales.

### Business Problem: 

Maverik, a convenience store and gas station chain with 300+ locations in the Western United States, aims to enhance its ability to assess the return on investment (ROI) for new stores, which are opened at an average rate of 30 per year. To achieve this, they require a new model capable of generating daily sales projections for merchandise, food sales, and total gallons sold for diesel and unleaded fuel for the entire first year of a store's operation.

This data-driven approach will enable Maverik to closely monitor the performance of new stores, make informed decisions, and promptly address any under performing outlets. Maverik desires to know the daily sales for each of the 4 main products diesel fuel, unleaded fuel, merchandise, and food sales. Having these daily predictions allows for better planning for seasonality and setting realistic goals and expectations for what each new store can bring in revenue for the year.

### Analytic Problem: 

The target variables is specifically daily sales for the diesel, unleaded fuel, merchandise, and food services. Represented in the time_series_data_msba.csv sets of time series sales data where the variables

daily_yoy_ndt.total_inside_sales: Inside sales, everything that isn't made at the store
daily_yoy_ndt.total_food_service: Food service sales, everything that is made at the store
diesel: Diesel gallons sold
unleaded: all non-diesel gallons
The main level of accuracy that we will use to determine the performance of this model is RMSE and R Squared.

Predict the daily sales for each 4 products diesel, unleaded fuel, merchandise, and food service for each store for the following year based on the time series data.

Use a Prophet method to see the daily sales predictions for each of the 4 product categories for a new store.

The success of this project will be measured by its capacity to accurately predict sales metrics and its usability for future stores. Our team will be judging our model based on RSME results. Since our target variables are numeric, we will explore which data features are significant via a linear regression model and then apply those features to a variety of data modeling techniques including a time series model.

### Solution to the Business Problem:



### The Business Value of the Solution:



### My Individual Contribution: 

I built the linear models to see if any of the variables in the dataset were significant and then applied that information as much as possible to my four Prophet models. The Prophet models aggregate the entire combined datasets while capturing daily, yearly, and holiday seasonality. Each Prophet model then predicts future sales for a single target variable for a single store. Tuning the models and testing each store on each model was a time intensive activity. I also compiled the three separate notebooks into this single group notebook for the group modeling assignment.

### Difficulties That My Group Encountered Along the Way:



### What I Learned in the Project:

I learned a considerable amount working on this project. 
