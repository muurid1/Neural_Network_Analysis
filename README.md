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

### Optimize the Model
