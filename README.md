# Neural_Network_Charity_Analysis

## Overview and purpose of the analyis: Explain the purpose of the analysis
This project was completed in 3 parts. First the charity dataset was preprocessed for Neural Network Model. Using the TensorFlow, a neural network is designed to create a binary classification model that can predict if an Alphabet Soup funded organization will be successful based on the features in the dataset. In the third part, the model is optimized to achieve a target predictive accuracy higher than 75%.
The purpose of the analysis is to use machine learning and neural network model to make prediction on whehter the organization will be successful if funded by Alphabet soup. 

## Results: Using bulleted lists and images to support your answers, address the following questions.

### Data Preprocessing

####   What variable(s) are considered the target(s) for your model?
The target variable for the model is "IS_SUCCESSFUL".

####   What variable(s) are considered to be the features for your model?
The feature variables for the model are "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE, "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT"

####   What variable(s) are neither targets nor features, and should be removed from the input data?
"EIN" and "NAME" variables are neither targets not features and should be removed from the input data.


### Compiling, Training, and Evaluating the Model

####   How many neurons, layers, and activation functions did you select for your neural network model, and why?
The first layer has 80 neurons and Sigmoid activation function is used. For second layer 30 neurons are used and Relu activation function is used. There is 1 output node in the model because the model is binary classifier and predicting either True or False outcome. The second layer has almost half number of neurons compared to layer one to reduce the computation time and relu function.

![Activation Functions](https://user-images.githubusercontent.com/103617509/195516581-f2e1cff7-4fc6-434f-b25f-3e963860a57f.png)

####   Were you able to achieve the target model performance?
No. The target level was 75% and achieved level is 46%

####   What steps did you take to try and increase model performance?
There were three steps taken to increase the performance of the model.
1) Increase Epochs from 100 to 150
2) Changing Activation Functions
3) Dropping more non-beneficial columns

![Activation Functions_Optimized](https://user-images.githubusercontent.com/103617509/195516583-cafcbd4a-6025-4848-8753-aee80618eebd.png)

## Summary:
For the original model, "Sigmoid", "Relu" and "Linear" activation function was used for first and second hidden layers and output layer respectively. The accuracy was noted to be 46%. In order to increased the performance, the epochs was increased from 100 to 150. Doing this didn't make much difference in the accuracy which increased to 47%. Second option was to changes the activation functions. I used "Relu" function for both hidden layers and "Sigmoid" function for output layer. The epoch was changed to 100 from 150. The accuracy was increased to 68%. Lastly, I dropped more non-beneficial columns. "STATUS" and "SPECIAL_CONSIDERATIONS" columns were removed. The accuracy was noted as 56% which is more than original model but less than the accuracy achieved from changing the activation functions. 
