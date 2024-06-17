# UK-Road-Safety-Analytics
RoadSafe Analytics is a comprehensive data science project focused on analyzing UK road safety data from the past five years. The project leverages advanced data processing and visualization techniques to provide insightful reports and dashboards aimed at understanding and mitigating serious roadside accidents. This project employs Azure PaaS Database for data storage and management, Microsoft Power BI Report Builder for creating detailed reports, and Power BI Dashboard for interactive data visualization.

## Data Sources and Preparation:

### The project utilizes three primary datasets:

- **Road Accidents Data:** Contains detailed records of road accidents, including date, time, location, and severity.
- **Road Vehicles Data:** Includes information about vehicles involved in accidents, such as vehicle type, age, and damage extent.
- **Casualties Data:** Provides details on casualties resulting from road accidents, including severity, age, and role (driver, passenger, pedestrian).

The data was meticulously cleaned and prepared using SQL, ensuring consistency and accuracy before being imported into the Azure PaaS Database.

## Data Integration and View Creation:
To facilitate analysis, views combining relevant columns from the three datasets were created. These views allowed for efficient querying and reporting. For example:

- **Accident Severity View:** Combined accident details, vehicle information, and casualty data to analyze the severity and causes of accidents.
- **Weather Conditions View:** Linked weather data with accident records to understand the impact of weather on road safety.
- **Driver and Vehicle Analysis View:** Focused on driver demographics, vehicle age, and types to assess their roles in accident severity.

## Azure PaaS Database Setup:

### Database Creation:

- Creation of an Azure SQL Database with a structured schema to hold the accident, vehicle, and casualty data.
- Configuring database parameters for optimal performance, including tier selection (Standard/Premium) and setting up performance monitoring tools.

### Data Import and Table Creation:

- Importing datasets into Azure SQL Database using BCP (Bulk Copy Program) and Azure Data Factory for large-scale data.
- Creating relational tables with appropriate primary and foreign keys to establish relationships among datasets.

## Report Building with Power BI Report Builder:
Five detailed reports were created using Power BI Report Builder, each addressing specific analysis scenarios:

- **1. Driver Age and Accident Severity:** Analyzes the correlation between driver age groups and the severity of accidents.
- **2. Weather Impact on Accidents:** Examines how different weather conditions affect accident rates and severity.
- **3. Road Surface Conditions:** Investigates the impact of road surface types on accident occurrences.
- **4. Vehicle and Casualty Analysis:** Studies the relationship between vehicle characteristics, hit objects, and casualty severity.
- **5. Geographical Analysis:** Maps accident hotspots and evaluates local authority district data to identify high-risk areas.

## Data Science Techniques in RoadSafe Analytics

### Statistical Analysis:
Statistical analysis was employed to understand and quantify relationships between various factors and road accidents. The following techniques were specifically used:

#### Regression Analysis:

- **Objective:** To identify which factors (e.g., weather conditions, driver age, vehicle type) significantly influence accident severity.
- **Method:** Multiple linear regression was applied to the dataset, with accident severity as the dependent variable and factors such as weather conditions, time of day, driver demographics, and vehicle characteristics as independent variables.
- **Outcome:** The regression coefficients helped quantify the impact of each factor on accident severity, providing insights into which variables are most predictive of severe accidents.

#### Correlation Analysis:

- **Objective:** To explore the relationships between pairs of variables within the datasets.
- **Method:** Pearson and Spearman correlation coefficients were calculated to assess linear and non-linear relationships, respectively.
- **Outcome:** High correlation values indicated strong relationships, such as between poor weather conditions and higher accident rates, guiding further in-depth analysis.

#### Hypothesis Testing:

- **Objective:** To test specific hypotheses about the data, such as whether the time of day affects accident severity or if certain vehicle types are more prone to severe accidents.
- **Method:** T-tests and chi-square tests were performed to compare means and distributions across different groups.
- **Outcome:** Statistical significance from these tests validated or refuted hypotheses, helping to identify critical risk factors for road safety.

### Machine Learning Models:
Machine learning models were developed to predict accident outcomes and segment the data for deeper insights. The following algorithms were used:

#### Regression Models:

- **Objective:** To predict the severity of an accident based on various factors.
- **Method:** Linear and logistic regression models were trained using features such as weather conditions, road surface types, vehicle age, and driver demographics.
- **Outcome:** The models provided probability scores for accident severity, allowing for early identification of high-risk scenarios and informing preventive measures.

#### Clustering Algorithms:

- **Objective:** To segment accident data into meaningful clusters for better understanding and targeted interventions.
- **Method:** K-means clustering and hierarchical clustering algorithms were applied to group accidents based on similarities in features like location, time, weather conditions, and vehicle types.
- **Outcome:** Clustering revealed distinct patterns, such as specific areas or times with higher accident frequencies, enabling focused safety campaigns and resource allocation.

#### Classification Models:

- **Objective:** To classify the outcomes of accidents, such as predicting whether an accident will result in fatalities or severe injuries.
- **Method:** Decision trees, random forests, and support vector machines (SVM) were employed, using features from the dataset to classify accidents into different severity categories.
- **Outcome:** These models helped in classifying accident severity with high accuracy, providing actionable insights for emergency response planning and policy-making.

## Application of Data Science Techniques in the Project

### 1. Regression Analysis:

- **Implementation:** The multiple linear regression model was implemented using Python libraries such as statsmodels and scikit-learn. The model was trained on a subset of the data and validated using cross-validation techniques.
- **Insights:** The analysis showed that poor weather conditions, nighttime driving, and certain road surfaces significantly increased the likelihood of severe accidents. These insights were visualized using coefficient plots and residual analysis charts.

### 2. Correlation Analysis:

- **Implementation:** Correlation matrices were computed and visualized using heatmaps in Python with libraries like pandas and seaborn.
- **Insights:** High correlations were observed between wet road conditions and accident frequency, and between driver age groups (e.g., young drivers) and accident severity. These findings helped prioritize which variables to include in predictive models.

### 3. Hypothesis Testing:

- **Implementation:** Hypothesis tests were conducted using scipy library functions for t-tests and chi-square tests.
- **Insights:** Significant differences were found in accident severity between day and night, and among different vehicle types. These results were presented in the reports to highlight critical risk factors.

### 4. Machine Learning Models:

#### Implementation:
- **Regression Models:** Linear regression and logistic regression were implemented using scikit-learn. Feature selection techniques, such as Recursive Feature Elimination (RFE), were used to optimize model performance.
- **Clustering Algorithms:** K-means clustering was performed using the scikit-learn library, with the optimal number of clusters determined by the elbow method and silhouette scores.
- **Classification Models:** Decision trees and random forests were trained using scikit-learn, with hyperparameter tuning performed using GridSearchCV.

#### Insights:
- **Regression Models:** Provided probabilistic predictions of accident severity, which were used to create risk maps and identify high-risk areas.
- **Clustering Algorithms:** Identified clusters of accidents with common characteristics, leading to targeted safety interventions in specific regions or under certain conditions.
- **Classification Models:** Classified accidents into severity categories with high accuracy, aiding in resource planning and emergency response strategies.

#### 5. Visualization and Reporting:

- **Implementation:** All statistical and machine learning results were visualized using Power BI and Python's visualization libraries (matplotlib, seaborn).
- **Insights:** Interactive dashboards and detailed reports presented the findings in an accessible format, allowing stakeholders to explore the data and make informed decisions.

## Road Accident Moniter in UK

![1](https://github.com/KavinduR0713/Child-Well-Being-Analysis-Ethiopia-and-Vietnam-in-/assets/105490780/bc5362a0-6445-43d8-8458-299f3eeb2459)

![2](https://github.com/KavinduR0713/Child-Well-Being-Analysis-Ethiopia-and-Vietnam-in-/assets/105490780/317613dc-088b-4acc-89f8-3e7525b52074)

![3](https://github.com/KavinduR0713/Child-Well-Being-Analysis-Ethiopia-and-Vietnam-in-/assets/105490780/0fc3a317-9154-455f-9e5c-a26ed1c7c400)

![4](https://github.com/KavinduR0713/Child-Well-Being-Analysis-Ethiopia-and-Vietnam-in-/assets/105490780/9d6b296a-2d70-4180-a07e-4140ad82f2f4)

![5](https://github.com/KavinduR0713/Child-Well-Being-Analysis-Ethiopia-and-Vietnam-in-/assets/105490780/8da20f56-23d4-4705-88fb-044802c9d998)

![6](https://github.com/KavinduR0713/Child-Well-Being-Analysis-Ethiopia-and-Vietnam-in-/assets/105490780/8c3b2fcb-f591-4462-972b-1e283062212c) 



## Conclusion:
RoadSafe Analytics is a powerful tool designed to provide valuable insights into road safety in the UK. By integrating advanced data science techniques with robust data management and visualization tools, this project aims to inform and influence policy decisions, enhance traffic safety measures, and ultimately reduce road accidents. The comprehensive analysis and interactive visualizations make it accessible for policymakers, researchers, and the public, driving data-driven decision-making in road safety initiatives.
