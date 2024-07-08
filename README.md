# deep-learning-challenge
This repository is to share my submission for the Deep Learning Challenge Homework. The coding in this repository was developed with the aid of our class activities and the xpert learning assistant.

Overview:

The purpose of this analysis is to help the nonprofit foundation Alphabet Soup select the applicants for funding with the best chance of success in their ventures. I have deployed a neural network model to help predict whether applicants will be successful if funded.

Results:

Data Preprocessing:

What variable(s) are the target(s) for your model?

Answer: The target variable for the model I used was the "Is_Successful" column. This column reflects which of the funded applications in the training data were successful and thus could be used to train the model to predict future successful ventures.

What variable(s) are the features for your model?

Answer: The features in my model were the remaining columns in the data set other than the target variable (the "Is_Successful" column) and the non-important variable (the "EIN" column).

What variable(s) should be removed from the input data because they are neither targets nor features?

Answer: The variable I removed as non-important was the "EIN" column.

Compiling, Training, and Evaluating the Model:

How many neurons, layers, and activation functions did you select for your neural network model, and why?

Answer: I used 2 hidden node layers with 80 and 30 nodes each (respectively) with the Rectified Linear Unit (ReLU) Function for activation. I settled on that model architecture as it yielded the target accuracy after I adjusted the preprocessing of the training data.

Were you able to achieve the target model performance?

Answer: Yes, after the steps I took to optimize my model it achieved an accuracy score of 79%

What steps did you take in your attempts to increase model performance?

Answer: I began my optimization by adjusting the model architecture by adding a third layer, changing the number of nodes for each layer, and changing the activation function for each hidden layer. I also tried adjusting the number of epochs.

Summary: 

After taking multiple steps to optimize the model itself it was only after adjusting the preprocessing of the training data to have it include the "NAME" column (and limit it to only those applicants whose name appeared 5 or more times) did I achieve the target accuracy. None of the steps I took to optimize the model had any significant effect on the models accuracy.

After working with the data, I would be interested in trying a Random Forest Classifier or Support Vector Machine to better predict successful outcomes. These models are adept at handling data sets like the one provided in this challenge that have both numerical and categorical variables, outliers, and data imbalances.
