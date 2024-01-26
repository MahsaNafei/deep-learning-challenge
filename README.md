# Alphabet Soup Deep Learning Model Analysis

### Purpose of the Analysis

The primary objective of this analysis is to develop a deep learning model using various architectures and configurations to predict the success of organizations funded by Alphabet Soup. The dataset, consisting of metadata for over 34,000 organizations, is processed and utilized to train and evaluate multiple neural network models. The analysis aims to achieve a high level of accuracy in predicting whether an organization will be successful or not, providing valuable insights for Alphabet Soup's funding decisions.

### Data Preprocessing

#### Target Variable
- Target variable(s) for the model: `IS_SUCCESSFUL`

#### Feature Variables
- Feature variable(s) for the model: `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, `ASK_AMT`, `NAME` (last model only)
  
#### Removed Variables
- Variable(s) removed from the input data: `EIN` and `NAME`

### Compiling, Training, and Evaluating the Models

#### Model 1
- Neurons, layers, and activation functions: 80 neurons in the first hidden layer (ReLU activation), 30 neurons in the second hidden layer (ReLU activation), 1 neuron in the output layer (Sigmoid activation).
- Target model performance: 72.61%


#### Model 2
- Neurons, layers, and activation functions: 160 neurons in the first hidden layer (ReLU activation), 80 neurons in the second hidden layer (Sigmoid activation), 20 neurons in the third hidden layer (Tanh activation), 10 neurons in the fourth hidden layer (Softmax activation), 1 neuron in the output layer (Sigmoid activation).
- Target model performance: 72.57%


#### Model 3
- Neurons, layers, and activation functions: 80 neurons in the first hidden layer (ReLU activation), 30 neurons in the second hidden layer (Sigmoid activation), 10 neurons in the third hidden layer (Tanh activation), 5 neurons in the fourth hidden layer (Softmax activation), 1 neuron in the output layer (Sigmoid activation).
- Target model performance: 72.77%


#### Model 4
- Neurons, layers, and activation functions: 14 neurons in the first hidden layer (ReLU activation), 7 neurons in the second hidden layer (ReLU activation), 1 neuron in the output layer (Sigmoid activation).
- Target model performance: 72.93%


#### Model 5
- Neurons, layers, and activation functions: 21 neurons in the first hidden layer (Softmax activation), 26 neurons in the second hidden layer (Softmax activation), 6 neurons in the third hidden layer (Softmax activation), 3 neurons in the fourth hidden layer (Softmax activation), 1 neuron in the output layer (Sigmoid activation).
- Target model performance: 72.86%

### Summary

The deep learning models exhibited varying performances, with Model 4 achieving the desired accuracy. Multiple attempts were made to optimize the models by adjusting input data, modifying neural network structures, and changing training regimens. The analysis demonstrates the complexity of predicting funding success and the importance of iterative model refinement.
