# Neural Network Charity Analysis

## Overview

Alphabet Soup's business team have provded a dataset containing more than 34,000 organizations that have received funding from the charity over the years.

Based on this dataset we plan to use machine learning and neural netwroks , to create models to predict whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing

Havng reviewed the initial dataset , is can be determined 👎

- The data provided shows a column for 'IS_SUCCESSFUL,' and will be the targeted data point for these predictions.
- The following data points (features) will be used as input for the models :- 
  - AFFILIATION
  - APPLICATION_TYPE
  - ASK_AMT
  - CLASSIFICATION
  - INCOME_AMT
  - ORGANIZATION
  - SPECIAL_CONSIDERATIONS
  - STATUS
  - USE_CASE

- The following data can be removed from the input data as they will have no direct effect on the model.
  - NAME
  - EIN

### Compiling, Training and Evaluating the model.

#### Initial Model

The initial model was created with 1 hidden layers with the activation function "RELU" and and output layer with the activation function "Signoid" with the first hidden layer having 80 neurons.

The target perfromance 75% was not met it was approximately 73% as can be see from the image below.

![Summary retiring](/Resources/Original_model.PNG)

[Link to initial model execution].

[Link to initial model execution]: https://github.com/JohnFortucci/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization_original.h5 

#### 1st test for improvement

To try an improve accuracy in the initial run , I added and additional hidden layers with the activation function "RELU" and reduced the number of neurons in the first layer by 10 , the second hidden layer has 40 neurons.

The target performance of 75% was not met , it was approximately 73%.

![Summary retiring](/Resources/first_optimization.PNG)

[Link to 1st improvement model execution].

[Link to 1st improvement model execution]: https://github.com/JohnFortucci/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization_opt_run_1.h5 

#### 2nd test for improvement

To try an improve accuracy in the initial run , I kept the 2  hidden layers with the activation functions "SIGMOID" and the second hidden layer with the activation function "RELU" with the first hidden layer having 80 neurons and the second layer having 30 neurons.

The target performance of 75% was not met , infact the accurcy reduced from the first run down by about 4% TO 66as can be seen from the image below.

![Summary retiring](/Resources/Initial_model_evaluation.png)
