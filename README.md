# Deep learning - project 1

# Image classification with convolutional neural networks

Autors: Agata Kaczmarek, Maciej Chylak

#### Theme of the project

In this project, we are going to implement different convolutional neural network architectures and use them in image classification problems. Then we will compare them to the built-in solution - ResNet18. We are also going to check the influence of hyperparameters change and data augmentation on the final effectiveness of the neural network. At the end, we will try to form a committee of neural networks.

#### Chosen technology

For this project, we are going to use the Python language and its library, which supports the creation of neural networks and work with them - PyTorch. It also allows users to work with both CPU and GPU, which will be useful for our project.

#### Comparison of neural network architectures

During this project, we will work with three different architectures of neural networks. At the end we will compare models we trained with pre-trained ResNet18, to check the differences in their performance. Architectures, which we will train, will be two more simple CNNs and ResNet18, but not pre-trained. The two simpler architectures were inspired by propositions of suitable models for the CIFAR 10 dataset.
Sources: [PyTorch website](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html?fbclid=IwAR0bHaGa9Ftgr0xu7-o1DQT_wSO7Z9iXrvTCwZjIDIU08HUOYHj44_NpEUQ), [CNN proposition](https://machinelearningmastery.com/how-to-develop-a-cnn-from-scratch-for-cifar-10-photo-classification/).

- simple convolutional neural network:
  - convolutional layer with ReLU as activation function interspersed with max-pooling layers two times,
  - flattening layer,
  - two fully connected layers with ReLU as an activation function,
  - fully connected layer.
- more complex neural network:
  - two layers each convolutional layer interspersed with max pooling and dropout layer three times,
  - flattening layer,
  - dense layer with softmax as an activation function.
- not pre-trained ResNet18
- pre-trained ResNet18 - to compare with other models

#### Influence of hyperparameters

During the work on our project we will investigate the influence of some hyperparameters on the results: 
- Related to training process:
  - Learning rate
  - Batch size
- Related to regularisation
  - The probability that the element will be zeroed for the dropout.
  - L2 regularisation
  
#### Data augmentation techniques

We will aim to make our models work better, that is why we will check the following data augmentation techniques:
- rotations
- horizontal flipping
- convert image to grayscale
- cutmix

#### Evaluation of solution:

Our solution will be evaluated with a ten-class confusion matrix. The main advantage of this metric is that it enables us to suspect the quality of the prediction for each class and allows us to find the class for which the predictions are weakest. Based on the results of the models we will investigate the influence of changes in hyperparameters and data augmentation. 

#### Ensemble of neural networks

After completing the above points and finding our best architecture for this problem, we will try the committee of neural networks. The aim will be to train a neural network on different subsets of data and with the use of voting choose the output of the ensemble. Later, we will compare the results with the ones obtained from single networks.








