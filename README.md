# Neural Network Charity Analysis

## Overview

Alphabet Soup's business team have provded a dataset containing more than 34,000 organizations that have received funding from the charity over the years.

Based on this dataset we plan to use machine learning and neural netwroks , to create models to predict whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing

Havng reviewed the initial dataset , is can be determined :- 

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

For all the model we ran 20 epochs for each model.

#### Initial Model

The initial model was created with 1 hidden layers with the activation function "RELU" and and output layer with the activation function "Signoid" with the first hidden layer having 80 neurons.

The target perfromance 75% was not met it was approximately 73% as can be see from the image below.

![Summary retiring](/Resources/Original_model.PNG)

[Link to initial model execution].

[Link to initial model execution]: https://github.com/JohnFortucci/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization_original.h5 

#### 1st test for improvement

To try an improve accuracy in the initial run , I added and additional hidden layers with the activation function "RELU" and reduced the number of neurons in the first layer by 10 , the second hidden layer has 40 neurons.

The target performance of 75% was not met , it was approximately 73% as can be seen from the image below. No major change from the previous model.

![Summary retiring](/Resources/first_optimization.PNG)

[Link to 1st improvement model execution].

[Link to 1st improvement model execution]: https://github.com/JohnFortucci/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization_opt_run_1.h5 

#### 2nd test for improvement

To try an improve accuracy previous models , I decided to change a number of variable to see if we could generate a change either positive or negative , kept the 2 hidden layers and chnaged the number of neurons in the first layer to 12 and in the second layer to six , I also changed the activation function function in the second hidden layer to "SIGMOID".

The target performance of 75% was not met , it was approximately 73% as can be seen from the image below. No major change from the previous models.

![Summary retiring](/Resources/second_optimization.PNG)

[Link to 2nd improvement model execution].

[Link to 2nd improvement model execution]: https://github.com/JohnFortucci/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization_opt_run_2.h5 

#### 3nd test for improvement

For the third improvement test added a third hidden layer , and adjisted the neurons and reverted all activation models to "RELU". Increased the neurons in the first layer to 140, increased neurons in the second layer to 20 and reverted to the activation model of "RELU". For the new hodden layer I configured the neurons to 15 and an activation model of "RELU"

The target performance of 75% was not met , it was approximately 73% as can be seen from the image below. No major change from the previous models.

![Summary retiring](/Resources/third_optimization.PNG)

[Link to 3rd improvement model execution].

[Link to 3rd improvement model execution]: https://github.com/JohnFortucci/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization_opt_run_3.h5

## Summary

- Initial run : 73.27%
- 1st Run     : 72.79%
- 2nd Run     : 73.24%
- 3rd Run     : 73.14%

## Model Recommendation

While the target of 75% was not met , we achieved approximately 73% across all models from this we could determine that while we did not achieve the 75% we where very close across all runs , this suggest that the model themseleves are good and therefore do not need changed.

In order the 75% we could investigate :- 
- The possibility of having additional datapoints.

