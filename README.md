# AirBnB_Analytics

The purpose of this project was to predict the prices of Airbnbs in Boston, along with it understand what features impact the price. <br>

Throughout this project, I will be focusing on the following questions:

- Is it possible to accurately predict the most attractive price of your Airbnb?
- What services will actually help you raise the price?
- What are the most favored neighborhoods?


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
RMSE is selected as the evaluation metric for this problem.<br>
**RMSE of our model = $41.25.**

<img src="https://github.com/Vaibhav3M/AirBnB_Analytics/blob/master/Analysis/Visualizations/rmse.png" height="300"/> 

But our main goal was to extract important features and understand what impacts price.
Feature importance parameters and visualizations were used for that purpose.
<br><br>

**SHAP value analysis:** <br>
SHAP values show how much each predictor contributes, either positively or negatively, to the price variable. This is like the variable importance plot but it is able to show the positive or negative relationship for each variable with the price.

<img src="https://github.com/Vaibhav3M/AirBnB_Analytics/blob/master/Analysis/Visualizations/SHAP.png" height="500"/> 
<br>

**Conclusion:**

- Predicting the exact price is difficult but many parameters impact the price and popularity of the place.
- Airbnb listing price is mostly determined by the type of house, location, number of bedrooms, and bathrooms.
- Amenities play a crucial role and are the best variable owner can play with to increase the rental value.
- People are willing to pay for Airbnb’s nearer to the city center.


For detailed result analysis read the below Medium article: <br>

**Medium post :**  https://medium.com/@malhotra.vaibhav0304/this-article-will-make-bostons-airbnb-hosts-rethink-their-investment-strategy-449df1a63830?sk=b87082484f163cc82e8873144c37c363

