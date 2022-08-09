# Forecasting-and-Survival-Analysis-Project
Key features: forecasting analysis- smoothening, moving average, exponential smoothening Business objective: Sales forecasting to be done in order to forecast the sales for the next few weeks given the dataset containing the sales on previous time periods. Survival Analysis to done on the type of the shipping mode to analyse the number of customers subscribing the ship mode from year 2001 to year 2012. How the diffetent types of shipping mode changes with time. Data Visualizations: Firstly, a proper study of the dataset is done, that is its data size, type of data, any null values and other very basic understanding of the datasets.  EDA- the number of null values are to be checked and there are 11 null values only in the postal code column which is very less compared on the entire dataset and hence are dropped. Plotting and understanding the sales trend as against the time column. the sales trend is positive and no seasonality. Various other plots are done such as understanding the sales of the products in terms of quantity and amount, most preferred mode for shipping against sales amount, number of product sold by category, sub-category, cities with highest sales and other plots to get the relation between the sales and the input features. Data Modelling: Now, various smoothing models are used and time series forecasting techniques to forecast the sales. Moving average is used. ACF and PACF plots are plotted to do the autocorrelation and partial autocorrelation plots. Simple Exponential Smoothing, Holt smoothing are done. The MAPE value is 95.123 and for the holt method it is 1972.82. Final model is done by combining bothe the training and testing models and then forecasting 10 future values. The model used is the Simple Exponential Smoothing. The ARIMA model is then used to train the model and test the accuracy on the testing data. The GridSearch model is done to obtain the p,d,q values for the ARIMA model, the p,d,q values are (2,1,0) .Then the test and train datasets are then combined and the model forecasts 10 future values. The forecast values and the available dataset is plotted with the forecast values plotted into the future. Survival Analysis The survival analysis is done on the shipping models, to check its subscriptions with date-time. The second and first class shipping mode fall with time to 20% survival and are mostly replaced by the standard class.  Important Features Selection: Then XGBoost Regressor model is used to fit the model and then is used to findout the best features. All the unnecessary features like postal-code, cusomter id, order date, row id , order id, etc are dropped. The rest of the models are encoded, to get labels for categorical data types. This data set is then fed as a training dataset with the sales column being the y value for the xgboost model and the important features are then plotted. As per the xgboost model the important features are: sub-category, category , region, state, city and segment in the descending order. 
