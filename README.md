# Neural_Network_Analysis

## Project Overview

The purpose of this project is to create a binary classifier capable to predict whether applicants will be successful if funded by Alphabet Soup. We will be using deep-learning neural networks with the TensorFlow platform in Python to help analyze and classify the success of charitable donations.

## Software:

• Python

• Jupyter Lab

• Pandas

• VS Code

# Data Source:

• [charity_data.csv](https://github.com/muurid1/Neural_Network_Analysis/files/9946312/charity_data.csv)

## Results

### Preprocessing Data for a Neural Network Model

#### What variable(s) are  considered the target for your model?

The target variable for the model is the "Is-Successful" column.

<img width="1252" alt="Screen Shot 2022-10-31 at 10 02 56 PM" src="https://user-images.githubusercontent.com/107282754/200183502-c7fbd3ea-0ffb-4c3c-9af6-3191d1f890a3.png">

#### What variable(s) are considered the feature(s) for your model?
The original model considered the following columns as features: NAME, APPLICATION, TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.

<img width="1217" alt="Screen Shot 2022-10-31 at 10 03 49 PM" src="https://user-images.githubusercontent.com/107282754/200183788-e89f64d5-70b7-4799-aef0-50eb6f7cbda5.png">

#### What variable(s) are neither and should be removed from the input data?
The employer Identification Number (EIN), the SPECIAL_CONSIDERATIONS and the STATUS were dropped.

<img width="517" alt="Screen Shot 2022-10-31 at 10 04 00 PM" src="https://user-images.githubusercontent.com/107282754/200184304-256c4a4b-a8a5-406c-8622-1f8506685de8.png">

### Compile, Train and Evaluate the Model

We have designed a neural network, or deep learning model, using Tensorflow in order to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset. We will figure out the amount of inputs there are and then determine the number of neurons and layers in the  model. Finally, we will compile, train, and evaluate the binary classification model to calculate the model’s loss and accuracy.

#### Neural network model with the number of input features and nodes for each layer using Tensorflow Keras.

<img width="887" alt="Screen Shot 2022-10-31 at 10 04 51 PM" src="https://user-images.githubusercontent.com/107282754/200186336-9cf99f30-e442-4f12-a74e-691517146475.png">

#### Evaluation of the model using the test data

<img width="745" alt="Screen Shot 2022-11-06 at 11 47 09 AM" src="https://user-images.githubusercontent.com/107282754/200186511-2797e0b8-3df8-4209-8145-c87a2834d12a.png">

##### How many neurons, layers, and and activation functions did you select for your neural network model, and why?

This model have three (3) hidden layers with many neurons for each because it seems to increase the accuracy above 75%.

##### Were you able to achieve the target model performance? 

Yes

##### What steps did you take to try and increase model performance?

• the conversion of the NAME column into data points, which has the biggest impact on improving efficiency

• the addition of a third layer and 

• the usage of the "sigmoid" activation function for the 2nd and 3rd layer.

### Optimize the Model

Optimization of  the model in order to achieve a target predictive accuracy higher than 75%

##### First_Attempt: Remove "SPECIAL_CONSIDERATIONS" from the dataset

<img width="640" alt="Screen Shot 2022-11-06 at 12 18 04 PM" src="https://user-images.githubusercontent.com/107282754/200188011-a76454b6-2aa5-4e45-95f1-31b94c55cb4c.png">

##### Second_Attempt: Adjustement of the amount of neurons and layers

##### Third_Attempt: Change of the output layer from "sigmoid" to "tanh"

• layer 1 : 80

• layer 2 : 60 

• layer 3 was added with the activation of "relu"

<img width="912" alt="Screen Shot 2022-11-06 at 1 06 52 PM" src="https://user-images.githubusercontent.com/107282754/200190092-f1c1b7c1-84cb-4ac2-ae22-50719d7d5f07.png">

## Summary

Overall, by increasing the accuracy above 75% we are able to correctly classify each of the points in the test data 75% of the time. And, an applicant has a 80% chance of being successful if they have the following:

The NAME of the applicant appears more than 5 times (they have applied more than 5 times)
The type of APPLICATION is one of the following; T3, T4, T5, T6, T7, T8, T10, and T19
The application has the following CLASSIFICATION; C1000, C2000, C3000, C1200, and C2100.
A good model to recommend is the Random Forest model because Random Forest are good for classification problems. Using this model produces a 78% accuracy.
