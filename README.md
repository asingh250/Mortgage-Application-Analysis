# Mortgage-Application-Analysis
Create a machine learning model which will predict if the mortgage will be approved or not based on 5 variables: age, income level, occupancy type, accepted, and debt-income ratio, Eliminating all the demographic bias except for age
We picked 5 attributes from the Mortgage data set provided and created a separate *.csv file to avoid extra data loss from the null values of the attributes which we neglect in our model.
We preprocessed the data to drop any null values of the applicants which might skew our datasets using the pandas library
For the processing part, we had some classification data with controlled intervals. We used Ordinal encoding to convert those into numeric discrete data for training and testing our model. We also had one, unique string data attribute, which was encoded using One-hot encoding to extract numeric values for processing.
With this clean data, we divided the data into two groups, 80% for validation and 20%, and trained our model to establish a correlation between mortgage application acceptance.


Using Matlab plot, we carried out data/representation/ visualization and found out, other than debt-to-income ratio, there isn’t any significant correlation between acceptance and other non-demographic factors
After this visualization to establish our hypothesis, we trained our model using the data set we created., and evaluate the model we created we applied 4 types of algorithms to test it out:
We used the Logistic Regression model to create a line the best fit for log-odds values to calculate the acceptance rate for the mortgage application. The F1 score, precision score, and recall score for this testing were very high, which suggested that the non-demographic factor which we accounted for didn’t have many roles in the application being accepted or rejected.
Similarly, we carried out a random forest model, Decision Tree, and Support Vector machine algorithm and each of those evaluations had really high precision, recall, and F1 score supporting the evidence from data visualization.
