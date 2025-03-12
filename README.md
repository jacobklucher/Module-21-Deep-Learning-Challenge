# Module-21-Deep-Learning-Challenge

## Overview of the Analysis

The purpose of this analysis was to build a machine learning model that can predict whether an organization funded by Alphabet Soup will be successful. This model aims to help Alphabet Soup in selecting applicants with the highest chance of success by analyzing the features of the given dataset and classifying applicants as successful or unsuccessful.

## Results

Data Preprocessing

* Target Variable:
  * The target variable is the "IS_SUCCESSFUL" column, a binary representation of whether the applicant was successful or not.
    
* Feature Variables:
  * The features include different data about each organization including application type, affiliation, classification, use case for funding, organization type, status, income, special considerations, and funding requested.
  * These features were used to predict the success for an organization.
    
* Variables To Remove:
  * The features that were removed were the EIN (identification number) and name of the organization.
  * These features are identification columns and do not contribute to the model's predictions of organization success.

Compiling, Training, and Evaluating the Model

* Model Architecture:
  * The neural network consists of three layers:
    * Layer 1: Hidden Dense layer with 4 neurons
    * Layer 2: Hidden Dense layer with 2 neurons
    * Layer 3: Output layer with 1 neuron providing binary classification of 0 for unsuccessful or 1 for successful
       
  * Activation Functions:
    * The hidden layers are using ReLU activation functions while the output layer is using Sigmoid
   
* Training Results
  * The model was trained for 100 epochs and improved significantly from beginning to end.
    * Epoch 1: Accuracy - 75.79%, Loss - 0.5687, Precision - 0.8428, Recall - 0.6554
    * Epoch 100: Accuracy - 99.96%, Loss - 0.0019, Precision - 1.0, Recall - 0.9993
   
* Model Performance
  
  * Final Evaluation:
    * The model met and exceeded the target performance, achieving very high values for accuracy, loss, precision, and recall.
    * The high accuracy and low loss values suggest that the model has effectively learned to classify the applicants into successful and unsuccessful categories.
      
  * Steps to Improve:
    * The model already shows high evaluation values, but further steps could be taken to improve the model more such as increasing the amount of epochs for training or tweaking the model layers. 

## Summary

The deep learning model performed very well, achieving almost perfect results in accuracy, loss, precision and recall. The model seemed to successfully learn to accurately predict whether an organization will be successful or not given the features from the dataset. A different model that could solve this problem just as well or potentially better would be a Random Forest model. Random forests usually have an improved accuracy rating compared to other models and it's less prone to overfitting due to the way a Random Forest model is made up of combining multiple decision trees. 
