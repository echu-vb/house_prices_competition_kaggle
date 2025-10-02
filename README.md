# Goal:
Predict the final sale price of 1459 houses from a test dataset via a machine learning model. Scores are evaluated based on the RMSLE of the model.

# Data Analysis
Within both the training and test dataset, there were no duplicates found. However, there was a high number of missing values with some columns having missing over 90% of the data. Columns with a very number number of nulls were dropped and the rest of the columns were imputed. A histogram was created to view the distribution of Sale Price which allowed me to see that the data was skewed to the right. This was solved by performing a log transformation on Sale Price and then reverting it back when making predictions. I then created a heatmap to view which features correlated most with Sale Price. Features like above ground living area and overall material/finish being the stand out features, having a correlation of over 0.7.

# Machine Learning
Between Random Forest and XGBoost, Random Forest was the winner from my testing. My final score with the hypertuned Random Forest Regressor was RMSLE=0.121.
