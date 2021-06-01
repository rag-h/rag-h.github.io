# Terminology
## Activation Function
Purpose: To introduce non-linearity into the network and to decide whether or not a neuron can contribute to the next layer.

How exactly do we determine whether or not a particular neuron can contribute?
Possible methods are:
1. **Step function**. Activate the neuron if its value is above a certain threshold. But this does not model every situation. Suppose we want classify neurons into three or more different categories. With the step function we can only have an activated neuron and a not activated neuron. We cannot classify these different neurons.
2. **Linear Function**. We can get a range of activations. The derivative of a linear function is constant. If we had connected layers, if all of them follow a linear function, the final layer will just be a linear function of the input layer. This means that the neural network can just be replaced by a single layer which can perform the same linear change. 
3. **Sigmoid Function**. This is what is commonly used. It is Non-linear. So combinations of this layer is are also non-linear. This function outputs an analog activation. The output of this function will be between 0 and 1, unlike the rages for the linear and step functions. It suffers from the vanishing gradient problem which means that if the input given is very large or small, it will squish it between 0 and 1.
4. **Tanh Function**. This is also known as a shifted sigmoid function. Non-linear. Range is from -1 to 1. This also suffers from the vanishing gradient problem.
5. **ReLu Function (rectified Linear Unit)**. Non-linear. Range goes from 0 to infinity, so it is non bounded. (I need to learn more about this. Still don't understand it properly).

### Why do we use non-linear functions? 
This is because no matter how many layers we have, if we have a linear function, it will become equivalent to having just one layer. 

## Loss Functions
A loss function is way to quantify the deviation of the predicted output to the expected output. There are several different types of loss functions as well. The choice of the loss function is determined by what project we are working on.

## Optimisers
During training, the parameters get adjusted to minimize the loss function to make our model as optimized as possible. The optimisers tie together the loss function and the different model parameters by updating the network in response to the loss function. They adjust the weight and the biases. The loss function fuides the optimiser. 
### Gradient Descent Optimiser
It is an iterative algorithm thats begins at a random point on the loss function and moves down its slope in steps until it reaches minimum point of the function. It is the most popular optimiser and it is fast, robust and flexible.
Algorithm:
1. Calculate what a small change in each individual weight would do to the loss function
2. Adjust the parameter based on its gradient (take a step in the determined direction)
3. Repeat steps 1 and 2 until we have the lowest loss function possible

The gradient here, is the partial derivative of all independant variables. When we do have high variable datasets the loss function can have several local minimas, but we need to find the global minimum. To do this, a proper **learning rate** is used. Taking steps that are too large or too small can hinder reaching the global minima. To make sure this doesn't happen a small number (usually 0.001) is multiplied to scale the gradients. This ensures that any changes made to the weights are quite small.

## Stochastic Gradient Descent
Instead of calculating the gradient descent for all input data, it is sometimes more efficient to caluclate this for just a subset of data. This is an implementation of the gradient descent that uses batches or random examples on each pass. It also uses something called **momentum** to accumulate gradients from the past steps to determine what might happen in the next steps.
Back propagation is gradient descent implemented on a network.

## Adagrad
- Adapts the learning rate specifically to individual features. 
- Some weights will have different learning rates
- This is ideal for sparse datasets with many missing input examples
- Learning rate tends to get smaller with time

## RMSprop
- This is a special version of Adagrad
- Accumulates gradients in a fixed window

## Adam
- Adaptive Movement Estimation
- Uses the concept of momentum
