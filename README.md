# Improve_MNIST_with_Convolutions
  Coursera : Introduction to TensorFlow for Artificial Intelligence, Machine Learning, and Deep Learning -  Week 3

We looked at how would improve Fashion MNIST using Convolutions.
For this exercise see if we can improve MNIST to 99.5% accuracy or more by adding only a single
convolutional layer and a single MaxPooling 2D layer to the model .
We should stop training once the accuracy goes above this amount. It should happen in less than
10 epochs, so it’s ok to hard code the number of epochs for training, but our training must end
once it hits the above metric. 
If it doesn’t, thenw e’ll need to redesign our callback.
When 99.5% accuracy has been hit, we should print out the string “Reached 99.5% accuracy so
cancelling training
A Conv2D layer with 32 filters, a kernel_size of 3x3, ReLU activation
function and an input shape that matches that of every image in the training set
- A MaxPooling2D layer with a pool_size of 2x2
- A Flatten layer with no arguments
- A Dense layer with 128 units and ReLU activation function
- A Dense layer with 10 units and softmax activation function


for TypeError: '>' not supported between instances of 'NoneType' and 'float'
 This error is similar to Exception with Callback in Keras - Tensorflow 2.0 - Python try replacing logs.get('acc') with logs.get('accuracy') Callback funcation

