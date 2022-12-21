# Neural_Network_Charity_Analysis

# Overview of the Project

With our knowledge of machine learning and neural networks, we’ll use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, we have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

__EIN and NAME__—Identification columns

__APPLICATION_TYPE__—Alphabet Soup application type

__AFFILIATION__—Affiliated sector of industry

__CLASSIFICATION__—Government organization classification

__USE_CASE__—Use case for funding

__ORGANIZATION__—Organization type

__STATUS__—Active status

__INCOME_AMT__—Income classification

__SPECIAL_CONSIDERATIONS__—Special consideration for application

__ASK_AMT__—Funding amount requested

__IS_SUCCESSFUL__—Was the money used effectively

# Analysis

### Preprocessing Data for a Neural Network Model

We need to preprocess the dataset in order to compile, train, and evaluate the neural network model.
Next, split the preprocessed data into features and target arrays.
Then split the preprocessed data into training and testing datasets.
Lastly, Standardize numerical variables using Scikit-Learn’s StandardScaler() class, then scale the data.

* What variable(s) are considered the target(s) for your model?

We need to analyze whether applicants will be successful if funded by Alphabet Soup. The column __IS_SUCCESSFUL__ values are considered as the target variables for the model which state if the money was used effectively by the organizations.

* What variable(s) are considered to be the features for your model?

All the other columns in the csv apart from __EIN and NAME__ are considered to be the features for your model.

* What variable(s) are neither targets nor features, and should be removed from the input data?

__EIN and NAME__ being the Identification columns are neither targets nor features and are dropped from the dataset before it is fit into the neural network model.

### Compile, Train, and Evaluate the Model

Using our knowledge of TensorFlow, we’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset. We’ll need to think about how many inputs there are before determining the number of neurons and layers in your model. Once we’ve completed that step, we’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.

* How many neurons, layers, and activation functions did you select for your neural network model, and why?

Selected 3 hidden layers, 60 units in hidden layer 1, 30 units in hidden layer 2 and 20 units in hidden layer 3. ReLu activation function for the hidden layer and Sigmoid activation function for output layer.

* Were you able to achieve the target model performance?

The model accuracy was 73% close to the target model performance.

* What steps did you take to try and increase model performance?

The large values in __APPLICATION_TYPE__ and CLASSIFICATION column were binned.
Total of 3 hidden layers were added to the neural network.
The epoch was increased to 200 to furthur train the model.

## Summary

The deep learning model had an accuracy of 73%.

The deep learning model is considered when the datasets are very large. For smaller datasets with a few thousand rows of data, the Logistic Regression model, SVM and Random Forest Classification model might predict with similar accuracy.  
