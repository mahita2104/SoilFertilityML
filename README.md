# SoilFertilityML
* This project investigates the predictive power of machine learning models in assessing soil fertility and its correlation with vegetation cover in . By using techniques like Random Forest(RF), Decision Trees (DT), Linear Regression, and simple ensemble methods, we develop models to predict soil fertility levels based on a range of soil properties.
* We found that soil properties vary depending on how we use the land. This matters because it can help us take care of the land better and deal with issues like pollution. Our research contributes to soil science and helps with farming, nature protection, and land management.
## Research Objectives
This project is guided by the following research objectives:

1. Development of Predictive Models: We aim to harness ML techniques, including Random Forest (RF), Decision Trees (DT), Linear Regression, and simple ensemble methods, to develop robust predictive models for soil fertility assessment.

2. Integration of Vegetation Insights: Recognizing the close relationship between soil fertility and vegetation, we seek to incorporate vegetation cover data and insights into our models. This integration will provide a more holistic understanding of the factors influencing soil health.

3. Practical Applications: Beyond model development, we investigate the practical applications of enhanced soil fertility insights. These applications extend to agriculture, nature protection, and land management, offering valuable tools for addressing real-world challenges.
## Dataset Description
This dataset contains the various elements found in the soil, for instance, organic matter, various nitrogen compounds, potassium, sodium, sulphates, boron, etc, It also contains various soil properties like pH. The target of this data is set to predict the vegetation cover which is the percent vegetative cover. The higher the vegetation cover higher is the fertility of the soil for crops. Vegetation cover is calcuated in percentage from 1 to 100, so, it becomes the regresion task. To achive the results various regression methods are applied and performance of each model is analysed.
## Data Preprocessing and Cleaning
A necessary step  to ensure that all the variables will be transformed to the same scale , all continuous variables contribute equally causing no biased results.
 - Imported Excel data into a Pandas DataFrame.
 - Handled missing values through imputation or removal.
 - Removed unnecessary rows and columns.
 - Renamed columns and attributes for clarity.
 - Assured length of column and attribute unit is same
 - Created a new dataframe with the following changes
 - Outlier Detection Using Boxplots:
   - Utilized boxplots to identify outliers in numerical columns.
   - Visualized data distribution, interquartile range, and outliers.
   - Considered different approaches for handling outliers as needed
## Exploratory Data Analysis
 - Data Visualization using pairplots
  ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Visualization_plots/pairplot.png)
 - Data Visualization using Heatmap
    - To find relationship between different attributes
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Visualization_plots/heatmap.png)
    - Vegetation Cover highly depends on pH

## Regression Techniques

 - Normalised the dataframe using MinMaxScaler to ensure that all features are on a similar scale.
 - Split the dataset into test and train dataset.
 - Implementing different ml models to access which model is best fit for this dataset.
 - ### Linear Regression
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Ml_Models_Plots/Linear_regression.png)
 - ### Decision Tree Regressor
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Ml_Models_Plots/Decision_Tree.png)
 - ### KNN regressor
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Ml_Models_Plots/KNN%20(1).png)
 - ### Bagging Regressor
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Ml_Models_Plots/Bagging_Regressor.png)
 - ### Random Forest Regressor
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Ml_Models_Plots/Random_forest.png)
 - ### Gradient Boosting
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Ml_Models_Plots/Gradient_Boosting.png)
 - ### Comparing Actual vs Predicted of all above models
   ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Comparison_Plots/ActualvsPredicted.png)
   
## Conclusion
- Comparing MSE(Mean-Sqaured Error) of all models
  ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Comparison_Plots/MSE(BEFORETUNING).png)
- Comparing MSE(Mean-Sqaured Error) after fine-tuning all the models
  ![](https://github.com/mahita2104/SoilFertilityML/blob/main/Comparison_Plots/MSE(AFTERTUNING).png)

  - KNN regressor and Gradient Boosting outperformed all the models with MSE less than 0.0004%
  - Linear Regression had the highest MSE
  - Due to small dataset we could attain such high precision but this causes lack of generalisation

