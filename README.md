# Fashion MNIST CNN Model

# Introduction

In this project, I have applied a Convolutional Neural Network (CNN) model to the Fashion MNIST dataset. The CNN model is a deep learning algorithm that is widely used for image classification tasks. The Fashion MNIST dataset consists of 70,000 grayscale images of 28x28 pixels size, each representing a fashion item from ten different categories. The goal is to classify each image into one of the ten categories.

# Data Preprocessing

I started by reading the train and test data files into a pandas dataframe. Then I converted the dataframes into float numpy because Keras accepts that and rescaled the pixels to values between 0 and 1 for better results while splitting them. I also split the data into a training set, a validation set, and a testing set using the train_test_split function from sklearn.model_selection.


# Data Visualization

I then visualized the data using matplotlib's pyplot package. I showed the first nine images of the training set with their corresponding labels, which were T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, and Ankle boot.


# CNN

I defined the image shape and the batch size and reshaped the data to fit the CNN model. I then built a basic CNN model in Keras with three layers: a convolutional layer, a max-pooling layer, and an output layer. The first layer in the model network, keras.layers.Flatten, transformed the format of the images from 28x28 2d array to a 1d array (of 28x28 = 784 pixels). I then compiled the model with a loss function, an optimizer, and metrics for accuracy.


# Results

After fitting the model on the training set and validating it on the validation set, I evaluated the model on the testing set. The accuracy of the model was 0.9071, which is quite good for a basic CNN model. However, the loss could be improved a bit.

#### Overall, this project demonstrates how to apply a basic CNN model to a dataset and achieve good results.
