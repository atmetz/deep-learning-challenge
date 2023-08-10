# deep-learning-challenge

## Analysis of Neural Network Model

# Overview:
This report will analyze the accuracy of using a neural network to predict if an applicant for funding will have a good chance of being successful if funded by Alphabet Soup.

# Results:
Data Preprocessing:
* The target vaiable in the data set is the IS_SUCCESSFUL variable.
* The features are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT.
* EIN, STATUS, SPECIAL_CONSIDERATIONS, and NAME variables were removed since they were neither targets nor features.

Compiling, Training, and Evaluating the model:
* I selected two hidden layers and one output layer, with the first input layer having 80 nodes and the second layer with 40 nodes. The first hidden layer used relu activation, the second hidden layer I used tanh, and the output layer used sigmoid.
* I was not able to reach the target accuracy number. With my optimization attempts I was able to get to 73.6% accuracy with the training data and 72.8% with the test data.
* I tried to remove some features that didn't seem to factor in the outcome of the project. Removing STATUS and SPRECIAL_CONSIDERATIONS gave the biggest improvement over the original model. I also adjusted the number of nodes in the second hidden layer and the activation.

# Summary: 
Overall, the attempts to optimize the neural network yielded minor improvements to the accuracy score. Since this is a yes/no classification, a supervised learning model might be able to get the desired accuracy target.