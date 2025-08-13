# Goal:
Predict the final sale price of 1459 houses from a test dataset via a machine learning model. Scores are evaluated based on the RMSE of the model.

# Data Analysis
Within both the training and test dataset, there were no duplicates found. However, there was a high number of missing values with some columns having missing over 90% of the data. All columns with missing values were dropped in order for the model to function properly. A histogram was created to view the distribution of Sale Price which allowed me to see that the data was skewed to the right but ultimately, the outliers were not dropped as the model lost accuracy fell from doing so. I then created a heatmap to view which features correlated most with Sale Price. Features like above ground living area and overall material/finish being the stand out feautres, having a correlation of over 0.7.

# Machine Learning
I used a Random Forest Regressor as my model and achieved an RMSE of 6536.067 and and R-squared of 0.993. This means that 99% of variance could be explained by my model.
