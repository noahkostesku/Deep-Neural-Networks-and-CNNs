## Project Description

In this project I implemented a deep neural network from scratch using Python and foundational libraries like NumPy and Pandas. This project demonstrates how to build a neural network step-by-step, including forward propagation, backpropagation, and model training, while incorporating advanced features like dropout, learning rate decay, and L2 regularization. 

## Dataset
I used the MNIST dataset, which contains 70,000 examples of handwritten digits. Each example is represented as a 28 x 28 grayscale image, flattened into a vector. The target variable y ranges from 0 to 9, corresponding to the digit labels.

## Features

`Forward Propagation`: Includes ReLU activation for hidden layers and softmax activation for the output layer.
`Backpropagation`: Calculates gradients for all weights and biases using matrix operations.

**Regularization**:

`L2 regularization`: Helps prevent overfitting by penalizing large weights. 
`Learning Rate Decay`: Exponentially reduces the learning rate over epochs for more efficient training.
`Batch Training`: Utilizes mini-batch gradient descent for faster convergence and improved optimization.
`Save and Load Model`: Serialize the model parameters using Python's `pickle` module for easy reuse.

## Mathematical Concepts
### 1. Initialization
`He Initialization`: Prevents vanishing and exploding gradient problems by stabilizing the variance of activations as they propagate through the network.

`Biases Initialization`: All biases are initialized to zero to avoid introducing initial bias into the model's predictions.

### 2.Forward Propagation

`Hidden Layer Activation`: Uses the ReLU (Rectified Linear Unit) function to introduce non-linearity and mitigate vanishing gradients.

`Dropout`: Applied to hidden layers during training to prevent overfitting by randomly deactivating a subset of neurons

`Softmax`: Computes class probability scores for the output layer.

### 3. Cost Function

`Cross-Entropy Loss`: Measures the difference between predicted probabilities and true labels.
`L2 Regularization`: Adds a penalty for large weights to the cost function to improve generalization.

### 4. Backpropagation

`Gradient Calculation`: Derives gradients of the cost function with respect to weights and biases using the chain rule.
`Learning Rate Scheduler`: Adjusts the learning rate dynamically during training for efficient updates.



