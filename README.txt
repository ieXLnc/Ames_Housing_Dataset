# Ames_housing_dataset

the Ames housing dataset is a classic dataset to practice data cleaning, feature engineering and various regression models in machine learning.
The dataset can be found [here](http://jse.amstat.org/v19n3/decock/AmesHousing.txt), and is composed of 2930 houses with 82 variables for each. 

My main goal was to create relevant features and models to demonstrate my skills in data processing and regression models.
My final model predicts house prices with an average absolute error of $11385. I also created a more robust stacked model that predicts (this time on 40% of the total data) with an MAE of $12385.41.

After finishing my models, I saw that this dataset was part of the Kaggle competitions (here) and adapted my code to be able to participate as well. I managed to finish in the top 9% of the leaderboard, a score I'm happy with.

The first file is the file for the cleaning of the dataset (missing data, outliers, features engineering) and the second one contains the different models and hyperparameters searches I did.

2 main discoveries on this dataset: the learning of the 'Optima' tool, a hyperparameter search tool that allowed me to refine my models and find more relevant parameters in much less time than the usual GridSearchCV on the biggest models - XGBoost, GradientBoosting. And also the 'mlxtend' module with the 'StackingCVRegressor' tool which allows to easily stack different models.