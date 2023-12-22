# Capestone Project

## 1. Walmart Stores Sales Forecasting
- **Project Title:**  Walmart Stores Sales Forecasting
- **Prepared for UMBC Data Science Master Degree Capstone by Dr. Chaojie (Jay) Wang**
- **Author Name:** Dheerajkumar Reddy. Appakondreddigari
- **Author's GitHub Profile:** https://github.com/dheeraj1027
- **Author's LinkedIn Profile:** https://www.linkedin.com/in/dheerajkumar-reddy-appakondreddigari-0182b2166/
- **Link to PowerPoint Presentation:** https://1drv.ms/p/s!AtllCB4q5RNGnxsqrWoLJQHqTyFu?e=7ya5Os
- **Link to YouTube Video:**  https://youtu.be/Yf4jRiaetp8 

## 2. Background
- Walmart is one of the largest retailers in the world, and its sales figures are a key indicator of
the health of the retail industry. 
- As such, forecasting Walmart's sales accurately is a crucial task that can help the company make informed business decisions and optimize its sales strategies
- Walmart's sales are affected by a wide range of factors, including store location, store type, department, holiday, temperature, and marketing promotions.
- To achieve this goal, this project will use the Walmart Store Sales Forecasting dataset from Kaggle and build a predictive model that can accurately forecast store sales. 
- This project can help Walmart identify the factors that affect store sales and potential opportunities to improve sales. 
- Using the mean absolute error metric to evaluate the accuracy of the sales forecasting model will allow us to determine how well the model performs in predicting actual sales.
- With an accurate sales forecasting model, Walmart can make more informed decisions about inventory management, staffing, and pricing. Ultimately, this can lead to improved sales and a stronger bottom line for the company.
- The Walmart Store Sales Forecasting dataset contains weekly sales data for 45 Walmart stores located in different regions across the United States. 
- The dataset includes data from 2010-02-05 to 2012-11-01. 
- There are- a total of 421570 observations in the dataset. 
- Each observation represents the sales for a specific department in a specific store for a specific week

## 3. Data
- **Data Sources:** The dataset is sourced from the Kaggle platform. it has 3 data sets in it
- **Link:** https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data
- **Data Size:** [4mb]
- **Data Shape:** [421570 rows and 16 columns ]
- **Time Period:** [February 2010 to December 2013]
- **Each Row Represents:** A sales history.

-  **Data Dictionary**
  
| Store | Date       | Temperature | Fuel_Price | MarkDown1 | MarkDown2 | MarkDown3 | MarkDown4 | MarkDown5 |     CPI     | Unemployment | IsHoliday |
|-------|------------|-------------|------------|-----------|-----------|-----------|-----------|------------|------------|---------------|-----------|
| 1     | 2010-02-05 | 42.31       | 2.572      | NA       | NA       | NA       | NA       | NA       | 211.0963582 | 8.106       | FALSE     |
| 1     | 2010-02-12 | 38.51       | 2.548      | NA       | NA       | NA       | NA       | NA       | 211.2421698 | 8.106       | TRUE      |
| 1     | 2010-02-19 | 39.93       | 2.514      | NA       | NA       | NA       | NA       | NA       | 211.2891429 | 8.106       | FALSE     |
| 1     | 2010-02-26 | 46.63       | 2.561      | NA       | NA       | NA       | NA       | NA       | 211.3196429 | 8.106       | FALSE     |
| 1     | 2010-03-05 | 46.5        | 2.625      | NA       | NA       | NA       | NA       | NA       | 211.3501429 | 8.106       | FALSE     |
| 1     | 2010-03-12 | 57.79       | 2.667      | NA       | NA       | NA       | NA       | NA       | 211.3806429 | 8.106       | FALSE     |
| 1     | 2010-03-19 | 54.58       | 2.72       | NA       | NA       | NA       | NA       | NA       | 211.215635  | 8.106       | FALSE     |

  - Potential Values: The potential values for categorical variables such as size, isholiday, etc., can vary widely and are determined by the actual data in the dataset. 
  - Target/Label Variable: weekly_sales
  - Selected Features/Predictors: yet to do

## 4. Exploratory Data Analysis (EDA)
- Conducted data exploration using Jupyter Notebook.
- Focused on target variables and selected features.
- Produced summary statistics of key variables.
  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/9f421d9d-63e5-4b7f-b97a-5889e63d97ad)
![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/cd7a82c1-c04a-4c31-a5ce-be37229cfdce)
![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/7088b61e-7e36-4065-a1ba-bb405998d426)

- Created visualizations.
  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/6bce4bf0-5edb-47bc-9b60-43a21834a080)
  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/fe16555a-1845-486c-afcc-1070a11e6c69)
  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/adda7782-961a-453c-a854-e4f6bc9b9a55)

  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/5ae7cd64-b000-445d-a9eb-7b8e3892fcd6)

- Checked for missing values and duplicate rows.
- Investigated the need for data splitting, merging, or augmentation.
  
  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/6411d0af-7e8f-47f5-a935-9e58b2f398f9)

- Explored the possibility of integrating other data sources.
  
- Pre-processed textual data if applicable.
- Ensured the resulting dataset is tidy.

## 5. Model Training 

  - **Predictive Analytics Models:**
  The following models will be employed for predictive analytics:
  - **Linear Regression**
  - Initially, we calculated the r2 scores for the test set which consists of 15 random stores.
  - Additionally, we calculated the R-squared scores for each store to identify the stores with the best, worst, and medium performance among them.

  - ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/c1655dae-1772-4639-9ce6-4f02ff49d03b)

    ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/4963cee7-47a4-40f7-8e10-1e958fdd4aed)

    ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/3b85101a-1fe2-4444-a285-7d590de71b85)


  - **KNN (K-Nearest Neighbors)**
  - **Time Series Analysis**
    The given time series data collection is assumed by the time series models to be stationary which means its mean and variance are both constant
    to determine whether or not the series is stationary we used the Augmented Dicky Fuller test
    As we can see that our p-value is definitely less than (0.5) and is even less than (0.01). So, we can say with pretty good confidence that we can reject the null (unit root, non-stationary data) and can assume our data is stationary
    
    Additionally, our ADF is much less than our (1%) confidence value of (-3.43), so we have another confirmation that we can reject the null hypothesis.
    ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/4fd1919e-d10c-463b-8fa0-72597cfec51f)

    ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/7b221708-1598-4889-98ad-391d7d307903)


- we chose Auto-ARIMA over ARIMA because it is difficult and time-consuming to find the ideal values for the number of Auto Regressors (p), number of Moving Averages (q), and Integrated (difference, d) in an ARIMA model. 
  


   ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/2397be1a-4ff4-42ff-b001-c8fbe57685a4)

  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/6b502793-467f-4201-8add-07aae7ba3776)
    
  - Random Forest
 ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/018ab758-fd52-4a00-a679-f5484b3138eb)
![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/390876f6-998b-4479-aadd-cf55a6b7dcd4)
![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/e2396cd4-690e-4e1c-8eed-c500c7824531)

  - XGBoost
  - ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/3fc3c8a2-42ca-4002-883a-24f9380e7db3)
  - ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/5df12d63-f386-4105-885a-67340a42e726)
  - ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/a91b7f4b-0e7c-40c4-81ea-7ba087be661c)

  - Decision Tree
    ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/324ae924-0f86-46bf-a954-ccdc48bc4648)
    ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/00b24583-6723-4751-a20e-f33232c27865)
    ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/18db3919-de24-49c2-9b46-29853704b972)




- **Model Training:**
  - **Train vs Test Split:** The dataset will be split into training and testing sets using an 80/20 ratio.
  - **Python Packages:** The models will be implemented using Python packages such as scikit-learn, etc.
  - **Development Environments:** The development environments for model training include your laptop, Google Colab, GitHub CodeSpaces, etc.

- **Performance Measurement and Comparison:**
- The performance of the models will be assessed and compared using relevant evaluation metrics, such as accuracy, precision, recall, and F1 score.
  It can be seen that the DecisionTreeRegressor model has a significantly high training R-squared score of 0.996, indicating that the model may be overfitting.

  The RandomForestRegressor and XGBoost models have relatively high R-squared scores for both training and testing sets, indicating that they may be performing well on the data.
  However, it's worth noting that the RandomForestRegressor model may also be overfitting slightly, as its training R-squared score is higher than the testing R-squared score. 

  Therefore, XGBoost seems to be performing best among all the models, as it has a high R-squared score on the testing set and a relatively low risk of overfitting.
  
  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/bc5f23c0-c4fa-4ed1-b2ec-0c4957df5efc)
  ![image](https://github.com/DATA-606-2023-FALL-TUESDAY/APPAKONDREDDIGARI-DHEERAJ/assets/113311883/3897f708-3c9a-4e63-a75b-148f9235ce0f)


## 6. Application of the Trained Models
- With an accurate sales forecasting model, Walmart can make more informed decisions about inventory management, staffing, and pricing. Ultimately, this can lead to improved sales and a stronger bottom line for the company

## 7. Conclusion
- In Conclusion, this study has evaluated the performance of a variety of supervised machine learning models, including linear regression, decision tree regression, random forest regression, and XGBoost models, on a dataset consisting of 45 stores. 
- We used 30 stores for hyperparameter tuning and 15 stores for testing. The results of our evaluation show that the XGBoost model achieved the best performance, with a training R2 score of 0.985 and a testing R2 score of 0.773.
- These results suggest that the XGBoost models. better suited than other models for the predictive tasks posed by this dataset.
- Overall, this study has shown that supervised machine learning models can be effectively used to perform predictive tasks on datasets such as the one used in this study.
- The results support the need for further research to explore the potential of supervised machine learning models in a variety of domains and datasets.
- Moreover, it is important to apply the results of these experiments to real-world applications, to explore the potential of this approach in practical settings
- After the train-test split, the results of the four regression models, Linear Regression DecisionTree Regressor, RandomForest Regressor, and XGBOOST showed that RandomForest Regressor performed the best with a Train _r2 of 0.99 and a Test r2 of 0.978.
- The DecisionTree Regressor also had a high Train_r2 of 1.0 and a Test_r2 of 0.963 Meanwhile, the Linear Regression and XGBoost had lower Train r2 and Test r2.
- This means that for the 45 stores of data, Random Forest Regression was the most effective model, followed closely by Decision Tree Regression
- This could create much better predictions, as the data that is provided can be used effectively. Additionally, the other two models, Linear Regression and XGBoost, could also be considered for further research as they could be further improved upon.
- Therefore, from these findings, it can be concluded that for creating predictions using the data of 45 stores random forest is the most suitable model

## 8. References
- Cheema, M. A., & Bhatnagar, A. (2021). Predictive analysis of sales forecasting using SARIMA models: A case of Walmart. Journal of Retailing and Consumer Services, 58, 102307.
- Fildes, R., Ma, L., Kolassa, S., & Huang, W. (2019). Demand forecasting with big data: A review. European Journal of Operational Research, 267(3), 1019-1033.
- Li, Y., Zhao, Z., Liu, C., & Huang, J. (2020). A neural network-based model for sales forecasting of Walmart. IEEE Access, 8, 63127-63135.
- Liu, H., & Liu, X. (2019). Store-level sales forecasting of Walmart: An application of Holt-Winters method. Journal of Retailing and Consumer Services, 48, 270-277.
- Miao, X., Chen, S., Liu, S., & Zhou, Y. (2020). A big data-based model for sales forecasting of Walmart. Complexity, 2020, 1-11.
- Yang, C., & Lin, J. (2019). Sales forecasting of Walmart using support vector regression. Journal of Retailing and Consumer Services, 50, 221-226.


