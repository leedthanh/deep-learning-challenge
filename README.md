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
I used binary_crossentropy for loss and adam for optimizer.

The model produced an Accuracy: 0.7262973785400391 which is below the target performance of 75% accuracy that I hope to achieve.  Therefore I used an optimized model by changing the number of neuron and hidden layers to get my model target to 75%.  

## Step 3: Build an optimized model to improve accuracy rate

I added another column feature NAME and increased another hidden layers to deepen the model neural network and as a result the optimized model produced an accuracy rate of 76% 
Here are the details of the optimized model.
First Hidden Layer: This layer has 30 neurons and uses the ReLU activation function. The ReLU activation function is a common choice for hidden layers as it helps the network learn complex patterns.
Second Hidden Layer: This layer has 20 neurons and also uses the ReLU activation function.
Third Hidden Layer:  This layer has 10 neurons and also uses the Relu activation function.
Output Layer: The output layer has 1 neuron and uses the sigmoid activation function.  The model is designed for binary classification tasks. The sigmoid activation function is commonly used for binary classification as it squashes the output into the range [0, 1], representing the probability of the positive class.  
I used binary_crossentropy for loss and adam for optimizer also 100 epoch.

# Summary
The model accurately predict 76% succesfull rate so I would recommend Alphabet Soup to use the model.  However, with more fine tunes the accuracy rate could improve with more hidden layers since deepen the network would help increase the accuracy.






 

