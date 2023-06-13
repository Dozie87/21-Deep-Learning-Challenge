# 21-Deep-Learning-Challenge
#Deep Learning with Neural Networks

#Analysis Overview
The purpose of this analysis is to assist the Non-Profit foundation, Alphabet Soup, by developing a tool that can help select applicants for funding with the best chance of success in their ventures. By using machine learning & neural networks, the goal of the analysis is to use various features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

#Data Preprocessing
#What variable(s) are the target(s) for your model?
The target for the model was the IS_SUCCESSFUL variable

#What variable(s) are the features for your model?
NAME
APPLICATION_TYPE
AFFILIATION
CLASSIFICATION
USE_CASE
ORGANIZATION
INCOME_AMT
ASK_AMT

#What variable(s) should be removed from the input data because they are neither targets nor features?
EIN
STATUS
SPECIAL_CONSIDERATIONS


#How many neurons, layers, and activation functions did you select for your neural network model, and why?
The details of the final chosen optimization model are listed below. Many combinations of layers were tested with varying nodes and the below yielded the best results.
(3) Hidden Layers
Layer 1: 66 nodes
Layer 2: 9 nodes
Layer 3: 3 nodes
(3) different activation functions: Tanh, Relu, Sigmoid

#Were you able to achieve the target model performance?

Yes, the final model performance had 78.71% accuracy. 
The goal was to achieve a model accuracy of over 75%

#What steps did you take in your attempts to increase model performance?
Adding/dropping various features to test the impact on the model.
Testing multiple unique values for cutoff points to bin "rare" categorical variables together
Changing the features used for binning
Testing multiple random_state values in train_test_split
Adjusting the number of hidden layers. Tested having 2,3, and 4 hidden layers with various counts
Trying different activation methods such as relu, para_relu, selu, tanh, and more
Adjusting the number of epochs
Using X_train_scaled in model instead of X_train Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
The initial deep learning model without any optimizations had an accuracy of about 73.04%


