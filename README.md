# Fake News Detection using LSTM Neural Network

This code is designed to demonstrate how to build a LSTM neural network for fake news detection. The dataset used in this code is the "Fake and Real News Dataset" available on Kaggle. This code makes use of various libraries such as numpy, pandas, matplotlib, seaborn and tensorflow.

The code starts by importing necessary libraries such as numpy, pandas, matplotlib, seaborn and tensorflow. It also imports the datetime module for date and time manipulations.

Then, it loads the dataset into pandas dataframes and preprocesses the data by concatenating the fake and true news dataframes, checking for null values, and combining the title and text column and dropping the title column.

Next, the data is split into training and testing datasets using the train_test_split() method from the sklearn library. The text data is then tokenized using the TextVectorization() method from the tensorflow library, which is then adapted to the training dataset.

The LSTM model is then built using the tensorflow library, compiled with the binary_crossentropy loss function and Adam optimizer. The model is then trained on the training dataset using the fit() method.

Finally, the model is evaluated using accuracy, recall, precision, and f1_score metrics from the sklearn library.