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
