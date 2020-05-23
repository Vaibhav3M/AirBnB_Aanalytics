# AirBnB_Analytics

The purpose of this project was to predict the prices of Airbnbs in Boston, along with it understand what features impact the price. <br>
**Medium post :**  

# Dataset 
Dataset : http://insideairbnb.com/boston/ 

## Libraries used:
- pycaret==1.0.0
- numpy==1.18.3
- pandas==0.23.4
- scikit-learn==0.22.2.post1
- matplotlib==3.0.3
- seaborn==0.9.1


# Files
 - **Analysis/Data-Preprocessing.ipynb**

The data through an ETL(Extract Transform Load) pipeline, which involved cleaning data, transforming data into a useful format, handling null values, etc, and finally store it into a CSV file for further use.

- **Analysis/Prediction.ipynb**

Pycaret library is used for predicting the price of Airbnb. 
This prediction is approched as a regression problem. CatBoostRegressor proved to be the best performing boosting algorithm for this problem.

# Results
RMSE is selected as the evaluation metric for this problem.
RMSE of our model = $41.25.

<img src="https://github.com/Vaibhav3M/AirBnB_Analytics/blob/master/Analysis/Visualizations/rmse.png" height="300"/> 

But our main goal was to extract important features and understand what impacts price.
Feature importance parameters and visualizations were used for that purpose.


