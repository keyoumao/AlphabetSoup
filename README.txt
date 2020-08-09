1. How many neurons and layers did you select for your neural network model? Why?
There are 54 inputs, 3 layers with 20 in the first layers, 10 in the second layer and 5 in the third layer. 
In the beginning, two layers of 20 and 10 neurons, respespectively, have been applied, but the accuracy was only 50%.
Then we gradually add layers and more neurons, and the final selction is a trade-off between the "too many" and "too few" neurons. Three layers are good 
for general scenarios.

2. Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
Yes. Four steps have been applied to optimized the model to match 75% accuracy.
1. Remove the noisy variables: 'EIN','CLASSIFICATION','APPLICATION_TYPE','STATUS'
2. Add additional neurons to hidden layers.
3. add additional hidden layers.
4. Try the other activation function, but doesn't show significant improvement.
5. Train with additional epochs, however, the convergence does not change too much after 100 iterations. 

3. If you were to implement a different model to solve this classification problem, which would you choose? Why?
Random forest tree. Because the data is tabular and the random forest requires less coding and computation resources. 