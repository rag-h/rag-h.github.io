# Introduction to Neural Networks
Neural networks form the basis of deep learning, which algorithms are inspired by the structure of the human brain. They take in data as an input, train themselves to understand the patterns in that data and then predict outputs for a new set of similar data.

A neural network consists of several neurons and three layers. The input later, the output layer and the middle hidden layer. There are generally several hidden layers between the input and output layers. 

![Structure of a neural network ](https://github.com/rag-h/rag-h.github.io/blob/master/blog/Deep-Learning/images/neural-network-structure.png)[Image Source](https://research.aimultiple.com/how-neural-networks-work/)

## How does a Neural Network Learn?
This can be broken into two processes. Forward propagation and back propagation.

### Forward Propagation
Flow of information from the input layer to the output layer. Neurons in the first layer connect to the next layer (first layer in the hidden layer) through channels. Each channel is assigned a numerical values called weights. The inputs are multiplied to the weights and their sum is sent as inputs to the hidden layer and each neuron in turn is associated to a numerical value called a bias. This bias is then added to the input sum. This input sum is then passed through to an activation function (a known non-linear function), which decides whether or not this neuron can contribute to the following layer. The output layer is a probability, where the neuron with the highest value determines what the output value is. 
### Back Propagation


### Sources:
1. https://www.youtube.com/watch?v=VyWAvY2CF9c

