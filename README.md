# forecasting_net_prophet

# Imports
1. prophet  -For forcasting
2. pandas - to read csv
3. holowviews - to plot data

# Istalations 
using google colab and install moules 
# Step 1: Find Unusual Patterns in Hourly Google Search Traffic
by reading csv using pandas library then plot search traffic for monthof may to see if there uneven fluctuations in out trend 

![bokeh_plot (2)](https://user-images.githubusercontent.com/69637182/187725647-e9b1f31e-2804-4919-94b5-c7c4c6d1b43a.png)

after make a comparesion between sum of search traffic and overall monthly median 

# Step 2: Mine the Search Traffic Data for Seasonality

plot different views by resample them by monthly, weekly and hourly then groupby them by index with using aggregation mean function 
![bokeh_plot (3)](https://user-images.githubusercontent.com/69637182/187726618-b27f770d-1266-43a0-9a64-5b211558e1de.png)


# Step 3: Relate the Search Traffic to Stock Price Patterns
In this section reading stock trend csv file, then plot close price showing bellow  
![bokeh_plot (4)](https://user-images.githubusercontent.com/69637182/187727700-3414c835-7976-40ff-b0e2-5dc81f161eff.png)

after we concate Search Trends with stock closing prices for only 6 month period of 2020 when market merged 

![bokeh_plot (5)](https://user-images.githubusercontent.com/69637182/187728563-8cf4a3ea-7d78-42f3-b2c6-a0fd595db7ae.png)
![bokeh_plot (6)](https://user-images.githubusercontent.com/69637182/187728596-eec9f257-b611-4a3e-9a51-3f3d55c73bff.png)

founding out both time series indicate a common trend 

After we added 3 more columns to our dataframe by making as shift of lag=1, lag=4 to lagged search trends, stock volatility respectivily and percent change of our 
closing prices to see if there correlation between them 
![bokeh_plot (7)](https://user-images.githubusercontent.com/69637182/187729562-91045609-f583-4d58-8320-e7f82fb78222.png)
![Screenshot 2022-08-31 112318](https://user-images.githubusercontent.com/69637182/187729597-dd517331-d504-4575-9996-04a8d6ac12d6.png)


 # Step 4: Create a Time Series Model with Prophet
 
Lastly making prediction of stock prices for the next 80 days by using Prophet on google coleb
reading csv dataset, then apply fbprophet model on out dataset after plot it make understanding of our stock behavior
![Screenshot 2022-08-31 112837](https://user-images.githubusercontent.com/69637182/187730692-ba68f707-f877-4534-a202-8a9bdf3c139f.png)
![Screenshot 2022-08-31 112903](https://user-images.githubusercontent.com/69637182/187730875-06869767-d969-463b-9842-d8606884b70d.png)


from last plot we see how search traffic behavios throught a year, week and day


