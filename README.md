# deep-learning-challenge
# Neural Network Model
## Overview of the analysis:
The purpose of this analysis is to build a machine learning model based on my knowdlege of machine learning and neural networks.
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures.  The Alphabet Soup dataset CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.  I Create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.
# Building the model 
## Step 1: Data Preprocessing
What variable(s) are the target(s) for your model?  As you can see in the Starter_code.ipynb I used IS_SUCCESSFUL variable as my target for the model.

Below are the features variables I used for my model.

APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested

I removed EIN and NAME because they are identification column

## Step 2: Compiling, Training, and Evaluating the Model
First Hidden Layer: This layer has 80 neurons and uses the ReLU activation function. The ReLU activation function is a common choice for hidden layers as it helps the network learn complex patterns.
Second Hidden Layer: This layer has 30 neurons and also uses the ReLU activation function.
Output Layer: The output layer has 1 neuron and uses the sigmoid activation function.  The model is designed for binary classification tasks. The sigmoid activation function is commonly used for binary classification as it squashes the output into the range [0, 1], representing the probability of the positive class.

The model produced an Accuracy: 0.7262973785400391 which is below the target performance of 75% accuracy that I hope to achieve.





 

