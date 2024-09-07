# neural_net_from_scratch

I'm currently learning about neural networks and will be documenting my progress by building them with just numpy on this GitHub repo as I go deeper into building better networks. Check out my other [repo]() where I reimplement ML papers in pytorch.

This network curently uses the `sigmoid function` as the activation function and the `cross entropy loss` as the cost function. The cross entropy performs better than the MSE/quadratic cost function because it 'fails fast'. Instead of taking small learning steps when model outputs are far from expected, it adjusts the weights and biases much quicker. 

I use a mini-batach stochastic gradient descent to minimize the loss function. I vectorized the backpropagation step to utilize numpy's efficiencies in matrix operations instead of backwardpassing for each individual neuron. This helped reduce the model training time.

### Updates
- Added the weight decay regularization penalty to the backpropagation step to reduce overfitting and improve model performance.
- Changed activation function from the `sigmoid function` to `relu`. The sigmoid compresses all neuron outputs to be within a range of [0, 1] however the relu activation function treats all negative outputs as zero and has no upper limit: [0, ∞]. In theory, this should help the relu work better and speed up up learning through faster convergence in gradient descent.

*Current Accuracy: 96.82%*

[Cost graph with ReLU](relu_cost.png)

[Accuracy graph with ReLU](relu_accuracy.png)

Up next: Convolutional Neural Network (CNN). This should work better than my current fully connected layer
