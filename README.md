# WiDs-Midterm
Winter in Data Science Project-- Computer Vision

In first week we discussed about python essential libraries such as pandas numpy, matplotlib. We discussed about activations functions such as tanh, ReLu, Softmax etc.
First week assignments consists of simple numpy and pandas operations, making numpy arrays, taking transpose of the array, ploting simple activation functions eg: tanh, Relu and softmax
2nd week's learning part consisted of regression algorithms and gradient descent the assignment was to make a logistic regression model for heart disease classification.
The Dataset given for the heart disease classification model had 15 features (eg. sex, age, smokes or not etc) and one column was for the possibility of heart disease ( 1 for Yes and 0 for no)
for the model I first cleaned the dataset it had some NA values that i had to deal with. Then i made a ClassificationModel class for the model
the classification model class has a constructor which make a list of weights having nin (number of features) elements and also randomely creates a bias
the call method runs when ever we call the model (class instance) it first takes dot product of the features_values with weights and sum up with bias and return the value operated over sigmoid function

the loss method takes the training/testing_values and training/testing_labels and run binery cross entropy error and returns the error value.
the step method does the one step gradient descent. it calculates the gradients of the weights and the bias then changes the values of weights and bias based on the gradients
method train calls the step method for 500 epochs, diagnos method tells us based on the sigmoid value whether the features results in heart disease or not ( if predicted value >=0.5 predicted labels = 1 otherwsie its 0) and at last the params method returns the list of weights and bias of our model

