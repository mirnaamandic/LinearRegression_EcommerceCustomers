"# LinearRegression_EcommerceCustomers" 

Exploratory Analysis: I used Python (pandas, seaborn, matplotlib) to summarize and visualize the data. Histograms and scatter/joint plots helped reveal relationships–for example, a joint-plot of membership length vs. spending showed a clear positive correlation(longer members tend to spend more).
I also examined correlations among features to spot potential multicollinearity or unexpected trends.

Data Preparation: I cleaned the data (e.g. dropping irrelevant columns like user ID or email) and ensured all predictors were numeric. Numerical features were standardized/normalized to help model convergence. Then I split the data into training and test sets to evaluate out of sample performance.

Model Training: I trained a linear regression model (using scikit-learn) on the training data. The model learned coefficients for each feature in the linear equation 
During training I also checked assumptions (e.g. residual plots) to ensure linear regression was appropriate.

Evaluation: I evaluated the model on the test set using metrics like R² (coefficient of determination) and RMSE (root mean squared error). The performance was quantified to see how well the model captured spending variance


**Results**

Model Fit: The linear regression model fit the data extremely well. It achieved a high R² (approximately 0.98) and a low RMSE (around 9–10 dollars) on the test set.
This indicates the model explains nearly all the variability in annual spending with the chosen features.

Key Predictors: Among the features, Length of Membership had the largest positive impact on spending. In fact, exploratory analysis and the fitted model consistently showed that customers with longer membership durations spent significantly more

App vs. Website Usage: Time spent on the mobile app was positively associated with spending. One analysis found each additional unit of app time raised yearly spending by about $38
. In contrast, time on the website showed little to no positive effect – it even had a slight negative correlation with spending in our data
. This suggests that engagement via the app drives more purchases than time spent browsing the site.




