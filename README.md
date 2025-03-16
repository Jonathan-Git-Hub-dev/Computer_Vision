Experimentation with Cifar100 and image recognition

Inspired by a somewhat recent addition to the iPhone that allows users to interact with their photo gallery, through searching the contents of the images by the objects it contains. 

Report:
This is a summary of the aim and implementation of the Model.

The general aim of the model is to be able to classify images containing single object so that it can be used in combination with other analogy or AI systems that break down larger images into candidates. These candidates can be processed individually to list the contents of complex images with multiple object.
The model will use the Convolutional Neural Network structure and be trained on the Cifar100 dataset with contains 60000 images split into 100 different categories. This data set will be further split into 3 groups, training, validation and testing so that the models training can be stopped when validation rises and tested on completely new data to get and accurate indication of performance.

 
Using a 3 layers of convolution, a pooling layer and finally 3 fully connected layers, the final training run resulted in a model with an accuracy of 30%. (The exact model architecture can be viewed in the Cifar100.ipynb notebook)

It is fair to say that performance improvements can be made. Through experimentation with different hyper parameters a much more accurate model can be reached, although I am unwilling at this time to do so as training runs take multiple hours.

Thank you for reading my model summary
