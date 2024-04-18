# SC1015-Mini---Project

Analysis for cardiovascular disease prediction through machine learning

# About:
In this mini-project, we look at a cardiovascular dataset consisting of various different variables.  
Mini-project by:
* Jarel Koh
* Boon Kiat
* Abineshkumar

# Background:
Cardiovascular Disease is the leading cause of death globally, representing 32% of global deaths.(World Health Organization: WHO, 2021)
Managing risk factors such as smoking and physical inactivity can significantly reduce the likelihood of developing cardiovascular diseases
# Objective:
We aim to predict cardiovascular disease risk using a dataset of health records from over 70,000 patients. The goal is to develop a machine learning model that is not only accurate but also practical. A health checkup in Singapore costs about 1.5k on average, hence with this model, we will help reduce the need for unnecessary health checkups, hence saving costs. The main aim of this project is to tell users whether they should or should not be going to a health checkup based on their risk of cardiovascular disease.
# What's Included:
1. Cardiovascular Dataset
2. Presentation Slides
3. Project Notebook
4.   * Data Preparation
     * Exploratory Data Analysis
     * Feature Engineering/Scaling
     * Machine Learning Models
         * Random Forest
         * K-Nearest Neighbours
         * Nerual Networks
     * Analysis
     * Conclusion
# Details about Notebook
## Data Preparation 
Our dataset consists of 13 features and over 70,000 records.  
1. Data Cleaning  
    * Redundant Column Removal: Columns not required for the analysis, such as 'id', were removed.
    * Outlier Detection and Removal: Outliers in critical health indicators, specifically in blood pressure measurements, were identified using physiological thresholds and removed to ensure data quality.
    * Data Transformation: Age data was converted from days to years to make the data more interpretable and relevant for analysis.
2. Data Visualization for Analysis  
We visually inspected the distributions of numerical attributes through boxplots to better understand their characteristics and verify the effectiveness of the cleanup process.

3. Feature Engineering  
We isolated categorical variables related to health and lifestyle choices into a separate dataset to facilitate detailed categorical analysis.

4. Model Data Preparation  
The dataset was split into training and testing sets to prepare for machine learning modeling, ensuring a balanced approach to training and validation.

## Exploratory Data Analysis
1. Data Visualization  
   * Box Plots: We used box plots to visually inspect the spread and outliers of numerical attributes. This was particularly useful for identifying extreme values in health measurements like blood pressure and body measurements.
   * Histograms: Histograms were employed to observe the frequency distributions of various attributes, helping to assess normality and skewness in the data.
   * Scatter Plots: We created scatter plots to explore potential relationships between variables. These plots were instrumental in spotting trends, correlations, and patterns that suggest relationships between different health indicators.
2. Correlation Analysis  
We conducted a correlation analysis to identify and quantify the relationships between different variables. This step was crucial for understanding which variables have potential predictive power and how they interact with each other.

3. Handling Missing Data  
Our analysis also included strategies for managing missing data, ensuring that our dataset was robust and our findings reliable. We explored the extent of missingness and evaluated different imputation methods where necessary.
## Machine Learning

## Analysis

## Conclusion

# What are the new things learned

# Contributions

# References


