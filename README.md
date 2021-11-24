# Deep-Learning-Homework
The non-profit foundation Alphabet Soup wants to create an algorithm to predict whether or not applicants for funding will be successful. With my machine learning and neural networks knowledge, I’ll use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
To do so the following steps has been taken:
work has been performed on Google colab

Import our dependencies 

Import and read the charity_data.csv.

Drop the non-beneficial ID columns, 'EIN' and 'NAME'.

Determine the number of unique values in each column.

Look at APPLICATION_TYPE value counts for binning

Choose 500 as cutoff value and create a list of application types to be replaced

used the variable name `application_types_to_replace`

Look at CLASSIFICATION value counts for binning

Choose 200 as cutoff value and create a list of classifications to be replaced

use the variable name `classifications_to_replace`

Convert categorical data to numeric with `pd.get_dummies`

Split our preprocessed data into our features and target arrays

 Split the preprocessed data into a training and testing dataset

Create a StandardScaler instances

## testing 
in 2nd testing changed classification and Application Types cut off values and it did not have much impact.
In 3rd testing increased a 3 rd layer which actualy decreces the efficiency.


 Fit the StandardScale

 Scale the data

### Compile, Train and Evaluate the Model

Define the model - deep neural net, i.e., the number of input features and hidden nodes for each layer.

Define input layer, 2 Hidden layers and output layers

nn_model.build()

Check the structure of the model

Compile the model

Train the model

Evaluate the model using the test data

Export our model to HDF5 file


testing one was done by changing cut off values and testing 3 rd is done by changing no of neuron and adding 3rd layer
but it can not achieve results more than 75 %.

