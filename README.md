# SoilFertilityML
* This project investigates the predictive power of machine learning models in assessing soil fertility and its correlation with vegetation cover in . By using techniques like Random Forest(RF), Decision Trees (DT), Linear Regression, and simple ensemble methods, we develop models to predict soil fertility levels based on a range of soil properties.
* We found that soil properties vary depending on how we use the land. This matters because it can help us take care of the land better and deal with issues like pollution. Our research contributes to soil science and helps with farming, nature protection, and land management.
## Research Objectives
This project is guided by the following research objectives:

1. Development of Predictive Models: We aim to harness ML techniques, including Random Forest (RF), Decision Trees (DT), Linear Regression, and simple ensemble methods, to develop robust predictive models for soil fertility assessment.

2. Integration of Vegetation Insights: Recognizing the close relationship between soil fertility and vegetation, we seek to incorporate vegetation cover data and insights into our models. This integration will provide a more holistic understanding of the factors influencing soil health.

3. Practical Applications: Beyond model development, we investigate the practical applications of enhanced soil fertility insights. These applications extend to agriculture, nature protection, and land management, offering valuable tools for addressing real-world challenges.
## Dataset Description
This dataset contains the various elements found in the soil, for instance, organic matter, various nitrogen compounds, potassium, sodium, sulphates, boron, etc, It also contains various soil properties like pH. The target of this data is set to predict the vegetation cover which is the percent vegetative cover. The higher the vegetation cover higher is the fertility of the soil for crops. Vegatation cover is calcuated in percentage from 1 to 100, so, it becomes the regresion task. To achive the results various regression methods are applied and performance of each model is analysed.
## Data Preprocessing and Cleaning
A necessary step  to ensure that all the variables will be transformed to the same scale , all continuous variables contribute equally causing that no biased results.
 - Imported Excel data into a Pandas DataFrame.
 - Handled missing values through imputation or removal.
 - Removed unnecessary rows and columns.
 - Renamed columns and attributes for clarity.
 - Assured length of column and attribute unit is same
 - Created a new dataframe with the following changes
## Exploratory Data Analysis
 - Data Visualization using pairplots
   

## Regression Techniques
## Conclusion
