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

