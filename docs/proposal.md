# Capestone Project

## 1. Walmart Stores Sales Forecasting
- **Project Title:**  Walmart Stores Sales Forecasting
- **Prepared for UMBC Data Science Master Degree Capstone by Dr. Chaojie (Jay) Wang**
- **Author Name:** Dheerajkumar Reddy. Appakondreddigari
- **Author's GitHub Profile:** https://github.com/dheeraj1027
- **Author's LinkedIn Profile:** yet to be done
- **Link to PowerPoint Presentation:** yet to be done
- **Link to YouTube Video:** yet to be done

## 2. Background
This dataset includes historical sales information for 45 establishments spread across several geographies. The aim is to project the sales for each department in each store, each of which has multiple departments. This can be achieved by using supervised learning algorithms such as linear regression, random forests, and decision trees. This will allow us to use the data to predict future sales and identify the most important features that are influencing sales.
## 3. Data
- **Data Sources:** The dataset is sourced from the Kaggle platform.
- **Link:** https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data
- **Data Size:** [4mb]
- **Data Shape:** [421570 rows and 16 columns ]
- **Time Period:** [February 2010 to December 2013]
- **Each Row Represents:** A sales history.

-  **Data Dictionary**
  
| Column Name       | Data Type           | Definition                                                  |
|-----------------------------------|---------------------|-------------------------------------------------------------|
| crash_date                         | Date and Time       | Date of the collision.                                     |
| crash_time                         | Date and Time       | Time of the collision.                                     |
| borough                            | String              | The borough in which the collision occurred (e.g., Manhattan, Brooklyn). |
| zip_code                           | String              | The ZIP code of the collision location.                    |
| vehicle_type_code1                 | String              | Type of the first vehicle involved.                        |
| vehicle_type_code2                 | String              | Type of the second vehicle involved.                       |
| vehicle_type_code_3                | String              | Type of the third vehicle involved.                        |
| vehicle_type_code_4                | String              | Type of the fourth vehicle involved.                       |
| vehicle_type_code_5                | String              | Type of the fifth vehicle involved.                        |
| contributing_factor_vehicle_1      | String              | primary contributing factor for the collision.             |
| contributing_factor_vehicle_2      | String              | Secondary contributing factor for the collision.           |
| collision_id                       | Unique Identifier    | Unique identifier for the collision.                       |
| vehicle_id                         | Unique Identifier    | Unique identifier for each vehicle involved.                |
| location                           | Geospatial Data     | Latitude and longitude coordinates of the collision.      |
| on_street_name                     | String              | Name of the street where the collision occurred.            |
| cross_street_name                  | String              | Name of the cross street.                                  |
| off_street_name                    | String              | Name of the nearest off-street location.                   |
| number_of_persons_injured          | Integer             | Number of people injured in the collision.                |
| number_of_persons_killed           | Integer             | Number of people killed in the collision.                 |

  - Potential Values: The potential values for categorical variables such as borough, vehicle_type_code1, contributing_factor_vehicle_1, etc., can vary widely and are determined by the actual data in the dataset. 
  - Target/Label Variable: yet to do
  - Selected Features/Predictors: yet to do

## 4. Exploratory Data Analysis (EDA)
- Conducted data exploration using Jupyter Notebook.
- Focused on target variables and selected features.
- Produced summary statistics of key variables.
- Created visualizations using Plotly Express.
- Checked for missing values and duplicate rows.
- Investigated the need for data splitting, merging, or augmentation.
- Explored the possibility of integrating other data sources.
- Pre-processed textual data if applicable.
- Ensured the resulting dataset is tidy.

## 5. Model Training
- Models for predictive analytics: [Specify the models to be used]
- Training methodology: 
  - Train vs test split: [Specify the split ratio]
  - Python packages: [Specify the relevant packages]
  - Development environments: [Specify the environments]
- Performance measurement and comparison methods: [Specify the metrics]

## 6. Application of the Trained Models
- Developed a web app for model interaction.
- Potential web app development tools: Streamlit, Dash, Flask.

## 7. Conclusion
- Summarized the project's work and potential applications.
- Identified limitations of the work.
- Highlighted lessons learned.
- Discussed future research directions.

## 8. References
- [List of references used in the project]
