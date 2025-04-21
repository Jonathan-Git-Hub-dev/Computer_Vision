Experimentation with Cifar100 and image recognition
Inspired by a somewhat recent addition to the iPhone that allows users to interact with their photo gallery, by searching the contents of the images. A user could enter “Car” into the search bar and only see the subset of their’ photos that contained this key word. 

The general aim of the model is to be able to classify images containing single object so that it can be used in combination with other analogy or AI systems that break down larger images into candidates. These candidates can be processed individually to list the contents of complex images with multiple objects. The model will use the Convolutional Neural Network structure and be trained on the Cifar100 dataset with contains 60000 images split into 100 different categories. This data set will be further split into 3 groups, training, validation and testing so that the models training can be stopped when validation rises and tested on completely new data to get and accurate indication of performance.

Using 3 layers of convolution, a pooling layer and finally 3 fully connected layers, the final training run resulted in a model with an accuracy of 30%. (The exact model architecture can be viewed in the Cifar100.ipynb notebook)
While I am moving on to other projects for a while, here are some things to consider if this project is revisited.
Because the number of hyperparameters configurations grows exponentially each time a new hyperparameter is considered it is very important to narrow down the areas of focus, here is an attempt to do so. When automatic termination on the rising of validation errors is turned off, training loss continues to shrink. This is good evidence that the model is overfitting not underfitting. This suggests that the model architecture and size have the potential to ‘solve’ this problem. To solve this problem I would focus on tools such as regularization and dropout.
Thank you for reading my model summary

