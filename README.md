# Neural_Network_Charity_Analysis

## Overview of the Analysis
### Using Machine Learning and Neural Networks for this project, I used the features in the dataset to create a binary classifier that will help predict if the applicants that will be funded by a Charitable organization called Alphabet Soup will be successful. We had a dataset containing various measures on 34,000 organizations that Alphabet Soup has supported for this analysis. This project compromised of the following three steps:
- Preprocessing the data for the neural network
- Compile, Train and Evaluate the Model
- Optimizing the model

## Results
### Data Preprocessing
- Variable that was considered as the target for my model: IS_SUCCESSFUL Column
- Variables that were considered features for my model: Every Column except for IS_SUCCESSFUL which is our target and the ones we will drop
- Variable that were neither targets or features for the dataset: Columns that I dropeed are EIN, NAME because they will have little to no impact om our outcome

## Compiling, Training and Evaluating the Model
### The number of neurons, layers, and activation functions I selected for my neural network model:
- For my neural network model I had 2 hidden layers. My first layer had 80 neurons, the second has 30 there is also an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

![191](https://user-images.githubusercontent.com/90746609/151891041-2c3df9d9-a21d-4c3b-ba67-82983fae6527.jpg)

### Was the model able to achieve the target model performance?

### The model was not able to reach the target 75%. The accuracy for my model was 69%.

![192](https://user-images.githubusercontent.com/90746609/151891418-484b2256-1e2d-41bf-adc8-28f02b467a22.jpg)

### The steps taken to try and increase model performance

### Attempt 1: Removed additional feature, that is the 'USE_CASE' column. Rest of the model components stayed the same, however model accuracy went down to 63%.

![193](https://user-images.githubusercontent.com/90746609/151892163-d42351fe-0bb4-4a8a-874c-98ba773bc5c8.jpg)

### Attempt 2: Adding Additional neurons to hidden layers and additional hidden layers are added. The accuracy went down again, this time it was 53%.
![194](https://user-images.githubusercontent.com/90746609/151892216-f081ead8-108a-45ac-9f1c-eca033a71974.jpg)

![195](https://user-images.githubusercontent.com/90746609/151892311-42ae0ad4-b59a-48ad-8b15-965a261c37d1.jpg)

### Attempt 3: Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model went down even more to 50%.

![196](https://user-images.githubusercontent.com/90746609/151892400-576fb3ab-83de-4e91-b69d-885190035ecc.jpg)

![198](https://user-images.githubusercontent.com/90746609/151892421-a711cf9b-ac67-441b-a73c-b374d018020e.jpg)


## Summary

### The model ended up with the accuracy score of 50% after optimization. The initial neural network had a accuracy score of 69%. This loss in accuracy can be explained from the fact that the model overfitted. Furthermore, we could further also optimize our neural network by removing more features or simply adding more data to the dataset to increase accuracy. Since our accuracy score was not particularly up to the standard with neural networks, we could have used the Random Forest classifiers. This is because random forest is a robust and accurate model due to their sufficient number of estimators and tree depth. Also the random forest models have a faster performance than neural networks and could have avoided the data from being overfitted.


