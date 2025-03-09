For this project, I decided to use multiple different tools to make my predictions for the web page attributes: length, word_present, and edited_2023.

First, I retrieved both the training and testing data from the links provided.

Then I created functions that I used to test and fit for regression. In the regression_test function I use a standard scaler to normalize the data and split the training data into training and testing via a 80-20 split. For evaluation, I use the sklearn metrics package to determine the score and MAE (mean absolute error) of the model -- this will help me decide which model to use on the testing data.

I create a similar function for binary classification where I also determined the confusion matrix. 

For **imputation** I used a simple imputer and replaced the NAN values with the mean.

For length, I tested several models - **linear, lasso, ridge, random forest, decision tree, elastic net, and a MLP regressor**. 


For word_present, I also tested several models and changed hyperparameters to see if there would be any improvement. I tested **logistic, random forest, and a MLP classifier**. 

For edited_2023, I first created a new dataframe with the training data and an added column with 0/1 values depending on if the file was edited in 2023. I later used logistic, random forest, and a MLP classifier as my models.


Below are the steps which I took whilst coding -- there are several internal comments and captions to provide further explanation to my thought process. 
