# Crypto To Wall Street Bitcoin Machine Learning
<p align="center">

<img width="190" alt="Bcoin" src="https://user-images.githubusercontent.com/96508478/180898343-791d1734-97f1-4f7b-934a-69fd1ac37d7d.png">

</p>

### At a Glance
Build a machine learning model to be able to accurately forecast future price of Bitcoin similar to that of the traditional stock market prediction.

### Data to Use and Question to Answer
Using historical bitcoin price data sourced from [Kaggle Bitcoin Historical Data](https://www.kaggle.com/code/smartsunny/starter-bitcoin-historical-data-1d758000-5/data) to perform an analysis on a Bitcoin dataset that provides the price and volume of trades of bitcoin everyday. 

Can we use the daily weighted average price and volume of trades to predict what the future of Bitcoin prices will be?

### Data exploration 
* Transformed and cleaned data with Pandas in Jupyter Notebook 
* Dropping null values 
* Set timestamp as our index

### Data Storage
After performing the transformation, the data is stored in a Postgresql database. 
In the Postgresql, we created 3 different tables
1. Bitcoin_trading
2. Bitcoin_prices
3. Bitcoin_movement

### Data analysis

* Bitcoin exchanges running from January 2016 through August 2019
* Columns in dataset include
  * Date: Used date as index
  * Open Price: Price at beginning of trading day
  * Close Price: Price at end of the trading day
  * High Price: Highest price for the trading day
  * Low Price: Lowest price for the trading day
  * Volume (BTC): Volume traded in Bitcoin
  * Volume (Currency): Volume traded in currency
  * Weighted Price: Price-weighted index

### Technologies, Languages, and Tools

* PostgreSQL
* Jupyter Notebook
* Pandas
* Tableau

### Machine Learning Models
* Random Forest Classifier
* Multiple Linear Regression
* Deep Learning
* SVM (Support Vector Machine)

To determine which model fit the data best, we will use metrics such as p-value, r-squared, accuracy, and loss.

---
### Bitcoin's Bull and Bear Market

Included in the visualizaition are the periods known as Bear and Bull markets.
 * Bear Market: Period of decreasing prices. Shown in red.
 * Bull Market: Period of increasing prices. Shown in green.

<img width="1112" alt="BearNBull" src="https://user-images.githubusercontent.com/96508478/182276029-2b2c5c82-9e72-4a20-bc40-721a4d9ee866.png">


---
### Price and Volume Correlation

Visualizing the relationship between the pricing and the volume of Bitcoin trading each year.

Using the blue color scale to demonstrate the elapsed time. The lighter cirlces represent earlier observations with the darker representing the latter.

1. 2017 Correlation Trendline:
Weighted Price = 179.99 * Volume + 2,245.69 

2. 2018 Correlation Trendline:
Weighted Price = 75.54 * Volume + 6,948.97

3. 2019 Correlation Trendline:
Weighted Price = 293.02* Volume + 4,576.70

We can observe a pattern based on the slope of the correlation lines. As the line get steeper, the price is rising at the same rate as the volume of trading. As the slope nears 0, the price is declining while the trading amount remains nearly the same, indicating sell off or Bear Market.

![AnnualPriceandVolumeCorrelation](https://user-images.githubusercontent.com/96508478/182276824-d829efca-a747-4a25-a859-1af08e289a37.png)


### Dashboard
Using Tableau to visualize data. To present our model information we will also show data using Python.

[Dashboard 1](https://public.tableau.com/views/AnnualPriceandVolumeCorrelation/Dashboard1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

[Dashboard 2](https://public.tableau.com/views/AnnualPriceandVolumeCorrelation/Dashboard2?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

[Google Slides](https://docs.google.com/presentation/d/1VHeZ6MnNOmpg_0YzP9D0KMj80vfIzco-kuI5W7_4aqA/edit#slide=id.p)
