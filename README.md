# WineQualityPrediction
Objective The primary goal of this project is to develop a machine learning model that can accurately predict the quality of red wine based on its physicochemical properties. The quality of the wine is classified into two categories: 'good quality' (quality score >= 7) and 'not good quality' (quality score < 7), making it a binary classification problem.

Data: The dataset comprises several observations of red wine, each characterized by the following features:

Fixed Acidity Volatile Acidity Citric Acid Residual Sugar Chlorides Free Sulfur Dioxide Total Sulfur Dioxide Density pH Sulphates Alcohol The target variable is 'quality', which is initially a score between 0 and 10. For the purpose of this project, we have transformed it into a binary classification problem, where wines with a quality score of 7 or above are labeled as 'good quality' (1), and the rest as 'not good quality' (0).

Methodology: The project adopts a structured approach to data analysis and model building, encompassing the following steps:

Data Exploration and Visualization: Initial steps involve exploring the data through various visualizations to understand the distribution of different features and their correlation with the target variable.

Feature Engineering: The creation of a new binary target variable 'goodquality' based on the existing 'quality' variable to facilitate binary classification.

Model Building: Utilizing Linear Regression as a predictive model. Given that linear regression outputs continuous values, a threshold is applied to convert its output to binary classes, facilitating classification evaluation.

Model Evaluation: Evaluating the model's performance using classification metrics such as accuracy, precision, recall, and F1-score. The focus is to achieve a balanced performance across both classes, with particular attention to improving the recall and F1-score for the minority class (good quality wines).

Preliminary Results The initial model has demonstrated the following performance metrics on the test data:

Accuracy: 86% Precision: 87% (for class 0) and 71% (for class 1) Recall: 99% (for class 0) and 11% (for class 1) F1-Score: 92% (for class 0) and 19% (for class 1) These results indicate a high accuracy but also suggest that the model is currently better at predicting the 'not good quality' class compared to the 'good quality' class, as evidenced by the higher recall and F1-score for class 0.

#Note- Doing this specific task with other algorithms may enhance the predictive model.

Implementation The project is implemented using Python, leveraging libraries such as pandas for data manipulation, seaborn and matplotlib for data visualization, and scikit-learn for building and evaluating the predictive model.

Conclusion By the end of this project, the aim is to have a predictive model that can accurately classify red wines as 'good quality' or 'not good quality' based on their physicochemical properties. The model's performance will be assessed using various metrics, with efforts directed towards enhancing the model's predictive accuracy, especially for the minority class, potentially through techniques like class balancing and feature engineering.

