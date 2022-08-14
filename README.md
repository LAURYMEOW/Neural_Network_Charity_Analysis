# Neural_Network_Charity_Analysis

## Analysis Summary:

The purpose of this analysis is to create a binary classifier that is able to predict whether applicants will be successful if they are funded by Alphabet Soup.
To achieve this, the deep neural network machine learning model methodology will be used.

## Results:

### Data preprocessing

- Which variable(s) are considered the target(s) for your model?

The target variable is 'Is Successful' since we are evaluating the success of the financing.

- What variable(s) are considered to be features for your model?

USE_CASE
APPLICATION_TYPE
AFFILIATION
ORGANIZATION
CLASSIFICATION
STATUS_1
ASK_AMT

- What variable(s) are neither targets nor features, and should be removed from the input data?

EIN
NAME
ASK_AMT

### Compiling, training and evaluating the Model

- How many neurons, layers and activation functions did you select for your neural network model and why?

The final model was specified with 4 layers:

* The first layer has 150 neurons and was selected with the Tanh activation function.
* The second layer has 150 neurons and was selected with the Tanh activation function.
* The third layer has 150 neurons and was selected with the Tanh activation function.
* The fourth layer has 100 neurons and was selected with the Tanh activation function.


### Image 1. Results for the optimized model

![](https://github.com/LAURYMEOW/Neural_Network_Charity_Analysis/blob/main/Resources/Summary_model.png)
![](https://github.com/LAURYMEOW/Neural_Network_Charity_Analysis/blob/main/Resources/Model%20evaluation.png)

The Tahn activation function was chosen since we have a wide input dataset and because the RELU function did not have a significant impact on the behavior of the model.

The model was run for 100 epochs, which is the recommended number of epochs to optimize a model of this type.

- Where you able to achieve the target model performance?

No
 
- What steps did you take to try and increase model performance?

* First I did a database check and decided to remove a variable that could be causing problems (INCOME_AIM).
* Create a new bin for rare occurrences for the column (ASK_AIM) and reduce the number of values for the other two bins so that they are left at 6 unique values each.
* Add more neurons to the model, then add more layers and change the activation function.
* I also added epochs to see if it improved the model but it didn't work and go back to 100 epochs.

## Summary 

It is difficult to achieve an acceptable accuracy with the current database with the implemented methodology.
Therefore, it is very likely that the model will be prone to overidentifying itself. It is pertinent to review the database, make a statistical analysis of the correlation of the variables and consider the variables of interest to the company.
It is also advisable to try another type of model, perhaps a less rigorous one such as supervised machine learning, since it is likely that a better result will be achieved in less time.
