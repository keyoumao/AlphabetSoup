# AlphabetSoup
Neuron Networks applied for successful prediction of the AlphabetSoup's project money usage.

## Introduction

From Alphabet Soup’s business team, a CSV containing more than 34,000 organizations that have received various amounts of funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization such as the following:
- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

## Algorithm and Methodology
Based on machine learning and neural network model building, we creatde a binary classifier that is capable of predicting whether or not an applicant will be successful if funded by Alphabet Soup using the features collected in the provided dataset. We build our own machine learning model that will be able to predict the success of a venture paid by Alphabet soup. The trained model was used to determine the future decisions of the company—only those projects likely to be a success will receive any future funding from Alphabet Soup.

**Established neurons and layers for the neural network model**

There are 54 inputs, 3 layers with 20 in the first layers, 10 in the second layer and 5 in the third layer. 
In the beginning, two layers of 20 and 10 neurons, respespectively, have been applied, but the accuracy was only 50%.
Then we gradually add layers and more neurons, and the final selction is a trade-off between the "too many" and "too few" neurons. Three layers are good for general scenarios. The trained model is given as follows.

![Neuron network model](https://github.com/keyoumao/AlphabetSoup/blob/master/Capture.JPG)

## Results and Discussion
**Model calibration and steps to improve the model performance**

Four steps have been applied to optimized the model to match 75% accuracy.
1. Remove the noisy variables: 'EIN','CLASSIFICATION','APPLICATION_TYPE','STATUS'
2. Add additional neurons to hidden layers.
3. add additional hidden layers.
4. Try the other activation function, but doesn't show significant improvement.
5. Train with additional epochs, however, the convergence does not change too much after 100 iterations. 

**Other models we have tried which have shown competency with the neuron network model.**

Random forest tree. Because the data is tabular and the random forest requires less coding and computation resources and runs faster than the neuron networks model, but the prediction accuracy is inferior. 


## Contact:
https://keyoumao.github.io/
