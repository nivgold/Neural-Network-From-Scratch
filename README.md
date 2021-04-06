# Neural-Network-From-Scratch
Implementation of a feed-forward neural network from scratch.

The implementation includes several sections:
---

* Forward Propagation - The forward propagation essential functions
* Backpropagation - The backpropagation essential functions
* Training Loop - The main training loop. As implemented, the network will learn as long as there is big enough (some epsilon value) improvement on a validation set.
* Regular Training Phase - Loading the MNIST dataset (from keras), splitting to training set and test set, and encoding the label with one-hot encoding. The network architecture used is as follows (input - most left, output - most right): input_size->20->7->5->10. The activation of the hidden layers is [ReLu](https://en.wikipedia.org/wiki/Rectifier_(neural_networks)) and [softmax](https://en.wikipedia.org/wiki/Softmax_function) for the output layer.
* Batch Normalization - Supporting a batch normalization layer (without the training parameters lambda and beta) and performing a training with batch normalization.
* Dropout - Supporting a dropout layer and performing a training with dropout. The dropout rate used is 0.2

The training configuration that was used in all of the experiments is:

> batch size: 64
 
> learning rate: 0.09

> improvement epsilon: 0.001
 
> max training iterations: 10,000

> 80% train and 20% validation ratio

The MNIST dataset that was used in the experiments: https://keras.io/api/datasets/mnist/
