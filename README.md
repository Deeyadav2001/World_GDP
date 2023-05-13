## GDP World Prediction

This project aims to predict the Gross Domestic Product (GDP) of different countries around the world. The dataset used in this project is 'gdpWorld.csv', which consists of data related to different countries such as population, birth rate, death rate, GDP, literacy rate, and many other factors. The goal is to use this data to train a machine learning model that can predict the GDP of a country based on its features.

### Requirements

This project requires the following libraries to be installed:
- numpy
- pandas
- seaborn
- matplotlib
- scikit-learn

### Dataset

The dataset used in this project is 'gdpWorld.csv', which consists of 227 countries and their respective features. The data preprocessing steps performed on the dataset are as follows:
- Replaced the string ',' with '.' as the float data cannot be separated by commas
- Checked data-types of the given data set
- Set data-types as float64 using ({'cols':'float64'})
- Checked for Missing values in the % format
- Filled the missing values or null values using mean and mode function
- Dropped the column of GDP to last columns to get the output

### Model Training and Testing

The data was split into training and testing sets, where 80% of the data was used for training and 20% was used for testing. The following features were selected for training the machine learning model:
- Phones (per 1000)
- Net migration
- Service
- Industry
- Crops (%)
- Infant mortality (per 1000 births)

A Linear Regression model was used to predict the GDP of different countries based on the selected features. The performance of the model was evaluated using the Root Mean Squared Error (RMSE), Mean Squared Log Error (MSLE), and R2 Score. 

Additionally, ElasticNet linear regression model was also trained and tested on the same features to see if it performed better than the Linear Regression model.

### Conclusion

The Linear Regression model achieved an RMSE of 5474.72 and an MSLE of 0.04 for the test data. The R2 Score for the test data was 54.08%, indicating that the model can predict 54.08% of the variation in GDP based on the selected features. The ElasticNet linear regression model, on the other hand, achieved an RMSE of 5699.25 and an MSLE of 0.04 for the test data. The R2 Score for the test data was 49.32%, indicating that the model can predict 49.32% of the variation in GDP based on the selected features. Therefore, the Linear Regression model performs slightly better than the ElasticNet linear regression model on this dataset.
