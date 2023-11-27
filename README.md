# Industrial-Copper-Modeling

Introduction
Elevate your expertise in data analysis and machine learning through our "Industrial Copper Modeling" project. Navigating intricate sales and pricing data in the copper industry presents unique challenges. Our solution leverages advanced machine learning techniques to tackle these complexities, providing regression models for accurate pricing predictions and lead classification to enhance customer targeting. This project will also hone your skills in data preprocessing, feature engineering, and the development of web applications using Streamlit, empowering you to effectively address real-world challenges in the manufacturing sector.

Key Technologies and Skills

Python
Numpy
Pandas
Scikit-Learn
Matplotlib
Seaborn
Pickle
Streamlit

Features

Data Preprocessing:

Understanding Data:
Before delving into modeling, it is essential to comprehensively understand the dataset. This involves identifying variable types, distinguishing between continuous and categorical variables, and examining their distributions. In our dataset, we may encounter unwanted values in the 'Material_Ref' feature, specifically those starting with '00000.' Converting these values to null enhances data integrity.

Handling Null Values:
Addressing missing values is a critical step in data preprocessing. The choice of handling null values, whether through mean, median, or mode imputation, depends on the data's nature and the specific feature.

Encoding and Data Type Conversion:
Preparing categorical features for modeling involves ordinal encoding, transforming categorical values into numerical representations. Additionally, ensuring data types align with modeling requirements is crucial.

Skewness - Feature Scaling:
Identifying and mitigating skewness in datasets is vital. The log transformation is a widely-used method to address high skewness in continuous variables, promoting a more balanced and normally-distributed dataset—often a prerequisite for machine learning algorithms.

Outliers Handling:
Outliers can significantly impact model performance. The Interquartile Range (IQR) method is employed to identify and adjust outlier data points, contributing to a more robust and accurate model.

Wrong Date Handling:
When dealing with delivery dates preceding item dates, calculating the difference and training a Random Forest Regressor model helps predict corrected delivery dates. This approach ensures data integrity and accuracy in the dataset.

Exploratory Data Analysis (EDA) and Feature Engineering:

Skewness Visualization:
To enhance data distribution uniformity, skewness in continuous variables is visualized and corrected using Seaborn's Histplot and Violinplot. The Log Transformation method is applied for improved balance and normal distribution while maintaining data integrity.

Outlier Visualization:
Outliers are identified and rectified using Seaborn's Boxplot. The IQR method is applied to bring outlier data points in line with the rest of the dataset, enhancing its resilience.

Feature Improvement:
Efforts focus on enhancing the dataset for more effective modeling. New features are created to gain deeper insights, ensuring dataset efficiency. Evaluation through Seaborn's Heatmap confirms no columns exhibit strong correlation, highlighting our commitment to data quality.

Classification:

Success and Failure Classification:
The 'status' variable is used to define 'Won' as Success and 'Lost' as Failure. Data points with status values other than 'Won' and 'Lost' are excluded for the core classification task.

Handling Data Imbalance:
To address data imbalance in the 'status' feature, the SMOTETomek oversampling method is implemented for a well-balanced dataset, enhancing classification performance.

Algorithm Assessment:
Various algorithms are applied to assess performance, and the Random Forest Classifier is chosen for its balance between interpretability and accuracy.

Hyperparameter Tuning:
GridSearchCV with cross-validation is employed for hyperparameter tuning, optimizing parameters for enhanced model performance.

Model Accuracy and Metrics:
The optimized Random Forest Classifier achieves 96.5% accuracy, with evaluation metrics providing a comprehensive view of its performance.

Model Persistence:
The well-trained model is saved to a pickle file, streamlining future applications.

Regression:

Algorithm Assessment:
For predicting the continuous variable of selling price, various algorithms are evaluated, and the Random Forest Regressor is selected for its balanced performance.

Hyperparameter Tuning:
GridSearchCV with cross-validation is used for hyperparameter tuning, optimizing parameters for improved model accuracy.

Model Accuracy and Metrics:
The optimized Random Forest Regressor achieves an impressive 95.7% accuracy, evaluated using key regression metrics.

Model Persistence:
The well-trained regression model is saved to a pickle file for easy loading and streamlined predictions in future applications.
