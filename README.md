# Neural_Network_Charity_Analysis

## Overview of the analysis
The purpose of this analysis is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

For this analysis, we are using a dataset containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.

## Results

### Data Preprocessing
* What variable(s) are considered the target(s) for your model?
The target variable is the column IS_SUCCESSFUL.

* What variable(s) are considered to be the features for your model?
The following columns are the features for our model: 
APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.

* What variable(s) are neither targets nor features, and should be removed from the input data?
The 'EIN'and 'NAME' are neither target nor features and should be removed from the input data.

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?

* Were you able to achieve the target model performance?

* What steps did you take to try and increase model performance?

Optimization #1:
Adjust the number of hidden layers to 6 and Nuerons to 30 between layers (initial 300). Keep the activation function as relu. At the end, the accurancy decreased in 0.4%.

Optimization #2:
Keep the data but adjust the number of hidden layers to 3 and Nuerons to 30 between layers (initial 300). There was an improvement of 0.2% in comparison to the first Optimization test. However, a decreased of 0.2% in comparison to the otiginal model.

Optimization #3
Adjust data(include STATUS), adjust the number of hidden layers to 4 and Nuerons(initial 130). Also, adjust the activation function to leaky_relu and Train the model in 200. In the end the model decreased in 0.2% in comparison to the original model and improved in 0.2% in comparison to test 1.

## Summary
The model did not reach the 75% expected. However, it can predict if applicants will be successful funded by Alphabet Soup with an accuracy of 72%.
It is possible to conclude that the data is too noisy and if we eliminate more features it may help improlbe the model. Also, a Random Forest may have a better prediction rate.