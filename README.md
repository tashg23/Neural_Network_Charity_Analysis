# Neural_Network_Charity_Analysis

## Overview: 
To help the charity Alphabet Soup determine whether applicants will be successful after receiving funding. 

## Results: 
### Data Preprocessing: 
1. We removed columns "EIN" and "NAME". 
2. Target variable = "IS_SUCCESSFUL"
3. The remaining columns are features in the model 

### Compiling, training and evaluating the model: 
We used 3 layers for this model. 

See image below for structure of the neural network: 
![NN Model](https://user-images.githubusercontent.com/113721712/234897850-80bb27f5-3e03-40ed-90bd-3f9488b09089.png)

The original model has an accuracy of 72%. 

### Model Optimization: 
First attempt: 
Added third hidden layer
New: 72% 

Second attempt: different activation function - from relu to tanh for first 3 hidden layers
New: 74% 

Third attempt: Increased number of bins for Classification column from 4 to 6. Increases input_dim from 41 to 43.
New: 74%

## Conclusion: 
Even after optimization, I was not able to achieve target model performance. Further tweaking would be needed. Overall, this neural network is 74% accurate for predicting whether a company will be successful after receiving funding from AlphabetSoup. Next steps could include trying out a different model, such as logistic regression. 
