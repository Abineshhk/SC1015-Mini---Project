# SC1015-Mini---Project

Analysis for cardiovascular disease prediction through machine learning

# About:
In this mini-project, we look at a cardiovascular dataset consisting of various different variables.  
Mini-project by:
* Jarel Koh @JarelKoh
* Boon Kiat @boonkiat014
* Abineshkumar @Abineshhk

# Background:
Cardiovascular Disease(CVD) is the leading cause of death globally, representing 32% of global deaths.
Managing risk factors such as smoking and physical inactivity can significantly reduce the likelihood of developing CVD.
# Objective:
We aim to predict CVD risks using a dataset of health records from over 70,000 patients. The goal is to develop a machine learning model that is not only accurate but also practical. A health checkup in Singapore costs up to 1.5k on average, hence with this model, we will help reduce the need for unnecessary health checkups, hence saving costs.
# What's Included:
1. Cardiovascular Dataset
2. Presentation Slides
3. Project Notebook
4. Data Preparation
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
    * Handling Missing Data: Our analysis also included strategies for managing missing data, ensuring that our dataset was robust and our findings reliable. We explored the extent of missingness and evaluated different imputation methods where necessary.
2. Data Visualization for Analysis  
We visually inspected the distributions of numerical attributes through boxplots to better understand their characteristics and verify the effectiveness of the cleanup process.

3. Feature Engineering  
We isolated categorical variables related to health and lifestyle choices into a separate dataset to facilitate detailed categorical analysis.

4. Model Data Preparation  
The dataset was split into training and testing sets to prepare for machine learning modeling, ensuring a balanced approach to training and validation.

## Exploratory Data Analysis
1. Data Visualization  
   * Box Plots: We used box plots to visually inspect the spread and outliers of numerical attributes. This was particularly useful for identifying extreme values in health measurements like blood pressure and body measurements.
   * Violinplot: We used violin plots, a combination of kde and box plot to show the distribution, probability density, and summary statistics of data, providing a comprehensive view of its underlying structure.
   * Countplot: We employed countplots to visually represent the frequency distribution of categorical data. 
2. Correlation Analysis  
We conducted a correlation analysis to identify and quantify the relationships between different variables. This step was crucial for understanding which variables have potential predictive power and how they interact with each other.

## Machine Learning Models
*  Random Forest: This ensemble model uses multiple decision trees to make a final decision, known for its high accuracy and ability to handle unbalanced data effectively. It's particularly useful in our context as it can handle the complexities of various risk factors involved in CVD without overfitting to the training data.
*  K-Nearest Neighbours (KNN): KNN was chosen for its ability to classify data based on feature similarity. This method is well-suited for our dataset as it can effectively find patterns in lifestyle and physiological data that are indicative of increased CVD risk. By examining the 'nearest' samples in the feature space, KNN can predict the patient's risk level based on similarities to known cases.
*  Neural Networks: Utilized for their capacity to learn non-linear relationships and complex patterns in large datasets. Neural networks are especially advantageous in predicting CVD because they can integrate various data types (like lifestyle habits, genetic factors, and clinical measurements) into a single predictive model, offering a holistic approach to risk assessment.
## Analysis  
Model Comparison: We evaluated each model based on its recall score to determine which is most effective at predicting CVD. This metric is essential in the medical field to ensure that the predictions are not only accurate but also minimize false negatives, which can be critical in a clinical setting.

Overall, we can conclude that:
*  Neural Network(Tensorflow Keras) is the best model for recall score and time taken to fit a mdoel.
*  K-Nearest Neighbours is the best model for time taken to predict using the model.

## Conclusion

*  All models perform similarly with its own strengths and weaknesses.
*  Although the fit time of Neural Network is longer than that of the K-Nearest Neighbors, and its predict time is higher than that of Random Forest, time is not an important factor for our problem. Our priority is to minimize the number of false negatives, and ensure the highest number of people with CVD are advised to get a checkup.
*  Thus, we conclude that Neural Network is the best model for our model.
*  For future improvements, we can perhaps create a dataset that is more localized to the context of Singapore to obtain better prediction for the Singapore population.

# What are the new things learned
*  Feature Selection
*  Recursive Feauture Elimination
*  Grid Search
*  Random Forest
*  K-Nearest Neighbours
*  Tensorflow Keras Neural Network

# References
*  https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset
*  https://pubmed.ncbi.nlm.nih.gov/30855814/#:~:text=Excerpt,is%20influenced%20by%20several%20variables.
*  https://www.tensorflow.org/guide/keras
*  https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html
*  https://www.ncbi.nlm.nih.gov/books/NBK11793/?report=reader
*  https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
*  https://scikit-learn.org/stable/modules/neighbors.html
*  https://www.harleystreet.sg/blog/benefits-and-costs-of-comprehensive-heart-screening/
*  https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.RFE.html

