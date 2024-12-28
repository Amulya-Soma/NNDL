This repository contains basic datasets that have been trained using various optimization algorithms. The code for each of these algorithms is written in a step-by-step mathematical manual calculation format, providing a clear and detailed implementation of the optimization process. The repository demonstrates the application of different gradient descent techniques to model training, allowing for a deeper understanding of how these algorithms work under the hood.


**Gradient Descent Optimization Algorithms**
These optimization algorithms are used to minimize the loss function in machine learning, adjusting model parameters to improve predictions. Below are the variations of gradient descent that enhance the basic optimization process.

1. Adagrad (Adaptive Gradient Algorithm)
Adagrad adapts the learning rate for each parameter based on the squared gradients accumulated over time. It helps in dealing with sparse data by adjusting the step size for each feature, reducing it when the gradient is large and increasing it when the gradient is small. However, it can lead to rapid decay in the learning rate, slowing down convergence in later stages.

2. RMSprop (Root Mean Square Propagation)
RMSprop is an improvement over Adagrad that uses an exponentially weighted moving average of squared gradients instead of accumulating them over all iterations. This helps maintain a more stable learning rate, preventing it from becoming too small. RMSprop is particularly effective for non-stationary objectives.

3. Momentum-based Gradient Descent
Momentum-based Gradient Descent adds a momentum term to the standard gradient descent updates. This term is a moving average of the past gradients, helping the model to "accelerate" in the relevant direction and reduce oscillations. It leads to faster convergence by smoothing out updates across iterations.

4. Nesterov Accelerated Gradient (NAG)
NAG is an enhancement to momentum-based gradient descent. Instead of using the current parameters for the gradient update, it uses the "lookahead" parameters—those that include the momentum term. This anticipates the future gradient direction and leads to more effective updates, often speeding up convergence.

5. Batch Gradient Descent
Batch Gradient Descent computes the gradient of the loss function using the entire training dataset in each iteration. The model parameters are updated only once per iteration based on the average gradient across all samples. While stable, it can be computationally expensive for large datasets, and its convergence may be slower compared to other methods.
