# deep-learning-challenge

The Alphabet Soup foundation has provided funding to over 34,000 organizations over the years. However, not all organizations have been successful in their ventures. the provided code using Machine Learning and ANN helps Alphabet Soup to select the applicants with the best chance of success in their ventures.

Model 1

What variable(s) are the target(s) for your model? 
IS_SUCCESSFUL (1) or Not (0) binary classification

What variable(s) are the features for your model?
APPLICATION_TYPE—categorical
AFFILIATION—categorical
CLASSIFICATION—categorical
USE_CASE—categorical
ORGANIZATION—categorical
STATUS—numerical
INCOME_AMT—categorical
SPECIAL_CONSIDERATIONS—categorical
ASK_AMT—Funding numerical

What variable(s) should be removed from the input data because they are neither targets nor features?
EIN and NAME—Identification columns

How many neurons, layers, and activation functions did you select for your neural network model, and why?
input : 43 based on X variables
Hidden layer 1: 80 - given (experimental)
Hidden layer 2: 30 - given (experimental)
output : 1 - binary cassification
functions: relu, relu, sigmoid

Were you able to achieve the target model performance?
With the first model I was able to get a 72.8% accuracy. However, I was not able to achieve the target model performance of 75% accuracy.

What steps did you take in your attempts to increase model performance?
To increase the model performance, I tried increasing the number of neurons and layers, changing the activation functions, and adjusting the learning rate. However, I still not reached 75%. 


Model 2 - optimized

What variable(s) are the target(s) for your model? 
IS_SUCCESSFUL (1) or Not (0) binary classification

What variable(s) are the features for your model?
APPLICATION_TYPE—categorical
AFFILIATION—categorical
CLASSIFICATION—categorical
USE_CASE—categorical
ORGANIZATION—categorical
STATUS—numerical
INCOME_AMT—categorical
SPECIAL_CONSIDERATIONS—categorical
ASK_AMT—Funding numerical

What variable(s) should be removed from the input data because they are neither targets nor features?
EIN and NAME—Identification columns

How many neurons, layers, and activation functions did you select for your neural network model, and why?
according to the defined function (makeDL model) I run a loop to find the optimum # of hidden layes and their neurans and here is the result:
{'activation': 'relu',
 'first_units': 10,
 'num_layers': 4,
 'units_0': 11,
 'units_1': 7,
 'units_2': 6,
 'units_3': 10,
 'units_4': 5,
 'units_5': 4,
 'units_6': 2,
 'units_7': 7,
 'units_8': 6,
 'units_9': 3,
 'units_10': 11,
 'tuner/epochs': 25,
 'tuner/initial_epoch': 0,
 'tuner/bracket': 0,
 'tuner/round': 0}

Were you able to achieve the target model performance?
With the first model I was able to get a 72.99% accuracy. It improved but did not achieve the target model performance of 75% accuracy.

What steps did you take in your attempts to increase model performance?
To increase the model performance, I loop between 0 to 10 layes of hidden layer including 0 to 10 neurons each layer. then reun every possibility to find the best model. Also, try different activation function. However, the best accuracy recived was I still not reached 75%. 
