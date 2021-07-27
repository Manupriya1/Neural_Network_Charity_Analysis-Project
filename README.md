# Alphabet Soup Charity Neural Network Analysis
## Overview
The purpose of this analysis is to use a neural network to decide which companies should recieve loans from Alphabet Soup. This analysis uses python's TensorFlow library to create, train, and evaluate data gathered from previous loans.

## Results
### Data Preprocessing
After looking at the data, I established that the target variable is the "IS_SUCCESSFUL" column. I then removed the "EIN" and "NAME" columns as they did not offer any relevant data that could help the model perform better. The remaining columns became the features for the model.

### Compiling, Training, and Evaluating the Model
- First attempt:  I used 8 neurons in the first layer and 6 in the second. I used relu activation functions for both and the output layer had a sigmoid activation function. Relu does better with nonlinear data, and two layers allows for a second layer to reweight the inputs from the first layer. Here are the preformance metrics of this model.
 <img width="330" alt="1" src="https://user-images.githubusercontent.com/69255270/127218069-d2e9cc07-9424-4e1c-9c55-4f47933a2703.png">

- Second attempt: I changed the activation function for the three layers to tanh to see if it makes the model better. 
<img width="303" alt="2" src="https://user-images.githubusercontent.com/69255270/127219933-8e5cdd6a-b45e-49b9-81a1-0118f0f71fc8.png">

- Third attempt: I changed the input layer to relu, output to sigmoid and the activation to tanh. Also changed the epoch to 500. 

<img width="328" alt="3" src="https://user-images.githubusercontent.com/69255270/127224401-afd3eb3e-3fd2-490e-a37e-ad60ee9983b0.png">


Summary
All three attempts mentioned above didn't improve the performance of the model and the accuracy remained less than 75%. I will continue to work to improve the model by reading more about the activation functions and how to choose them. and also modify the data by dropping some of the insignificant data like "status" and changing the threshold value. 
