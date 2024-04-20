# Project Summary: Influencer Comparison Model

## Objective
The goal of this project is to build a machine learning model that can predict which influencer out of a pair (A and B) is more influential based on various social media metrics. The predictions help in understanding the impact of influencers' online presence and can guide marketing and promotional decisions.

## Data Description
The dataset contains several features related to two influencers, labeled as A and B in each row. Each feature includes data like follower count, following count, number of times listed, mentions received, retweets received, mentions sent, retweets sent, and network features. The target variable Choice indicates which influencer is considered more influential (0 or 1).

## Data Processing
### The data was processed through several steps:
Exploratory Data Analysis (EDA): Included generating summary statistics, visualizing distributions with histograms, detecting outliers with box plots, and examining correlations.
Data Cleaning: Applied log transformations to reduce skewness and scaled numerical features using StandardScaler to standardize data for modeling.
Handling Outliers: Outliers were mitigated by applying log transformations to highly skewed distributions.
Model Development
Several machine learning models were trained and evaluated:

* Logistic Regression
* Random Forest
* Gradient Boosting Machine
* Support Vector Machines (SVM)
* Neural Networks

Gradient Boosting Machine provided the highest accuracy among initial models, but further experiments were conducted with different architectures and parameters, especially with Neural Networks to improve performance.

## Saving the Model
The Gradient Boosting Classifier was saved using pickle for later use in predictions, ensuring the model could be easily loaded and applied to new data without retraining.

## Prediction on Test Data
The test data was prepared using the same transformations as the training data. The model was then used to make predictions on this preprocessed test data. Predictions were saved to a CSV file for further analysis or deployment purposes.
