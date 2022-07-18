# Technologies Used

## Data Transformation and Cleaning
To preform the analysis on the bitcoin.csv file, we begin by transforming and cleaning our data with pandas in Jupyter Notebook.
We dropped any null values and set the timestamp as the index for our dataset.

## Data Storge
After preforming the tranformation, the data is stored in a Postgresql database. In the Postgresql, 3 different tables:
1. Bitcoin_trading
2. Bitcoin_prices
3. Bitcoin_movement


## Machine Learning Models
We have created 4 different machine learning models to run our data through to determine which model provides the highest accuracy score and lowest loss.

#### Steps
1. We are standardizing the bitcoin dataframe before using PCA to reduce dimentions to three principal components.
2. The elbow curve was utilized to determine the number of clusters in the data, then printed predictions.
3. Then the data is run through train_test_split(), then we run the linear regression model to weigh the effect of the independent variables.

## Dashboard
We are using Tableau to visualize our findings.
To present our model information we will also show data using python.
