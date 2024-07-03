# neural_net_from_scratch

I'm currently learning about neural networks and will be documenting my progress on this GitHub repo as I go deeper into building better networks.

This network curently uses the `sigmoid function` as the activation function and the `cross entropy loss` as the cost function. The cross entropy performs better than the previous MSE/quadratic cost function because it 'fails fast'. Instead of taking small learning steps when model outputs are far from expected, it adjusts the weights and biases much quicker. 

I use a mini-batach stochastic gradient descent to minimize the loss function. I vectorized the backpropagation step to utilize numpy's efficiencies in matrix operations instead of backwardpassing for each individual neuron. This helped reduce the model training time.


*Current Accuracy: 96.79%*
