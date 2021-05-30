# Terminology
## Activation Function
Purpose: To introduce non-linearity into the network and to decide whether or not a neuron can contribute to the next layer.

How exactly do we determine whether or not a particular neuron can contribute?
Possible methods are:
1. Step function. Activate the neuron if its value is above a certain threshold. But this does not model every situation. Suppose we want classify neurons into three or more different categories. With the step function we can only have an activated neuron and a not activated neuron. We cannot classify these different neurons.