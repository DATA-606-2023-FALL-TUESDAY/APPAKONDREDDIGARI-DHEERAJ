# New York City Motor Vehicle Collisions Analysis

## 1. Title and Author
- **Project Title:** New York City Motor Vehicle Collisions Analysis
- **Prepared for UMBC Data Science Master Degree Capstone by Dr. Chaojie (Jay) Wang**
- **Author Name:** Dheerajkumar Reddy. Appakondreddigari
- **Author's GitHub Profile:** https://github.com/dheeraj1027
- **Author's LinkedIn Profile:** yet to be done
- **Link to PowerPoint Presentation:** yet to be done
- **Link to YouTube Video:** yet to be done

## 2. Background
The New York City Motor Vehicle Collisions Analysis Project aims to provide valuable insights into motor vehicle collisions in New York City. This analysis is crucial for enhancing road safety and urban planning. The project seeks to answer questions such as the primary causes of collisions, high-risk areas, collision patterns over time, and the influence of weather and road conditions.
-The project seeks to address critical questions such as:
1. What are the primary causes of road accidents in New York?
2. Where are the high-risk zones for accidents within the state?
3. What specific times of day and days of the week witness a higher propensity for accidents?
4. How do different accident types (e.g., rear-end collisions, head-on collisions, sideswipes) vary in terms of frequency and severity?
## 3. Data
- **Data Sources:** The dataset is sourced from the New York City Open Data platform.
- **Link:** https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Vehicles/bm4k-52h4
- **Data Size:** []
- **Data Shape:** [3.7 million rows and 25 columns ]
- **Time Period:** [April 2016 to December 2021]
- **Each Row Represents:** A motor vehicle collision.

-  **Data Dictionary**
-  
| Column Name                       | Data Type           | Definition                                                  |
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
  - Target/Label Variable: [Specify the target variable]
  - Selected Features/Predictors: [Specify the relevant features]

## 4. Exploratory Data Analysis (EDA)
- Conducted data exploration using Jupyter Notebook.
- Focused on target variable and selected features.
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
