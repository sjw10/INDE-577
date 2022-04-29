# Multi-Layer Perceptron
The perceptron model we explored previously was the single Perceptron model. This meant that you put all your inputs into a single function to get a single output. However, for the multi-layer perceptron there are multiple layers with multiple nodes. The image below can help visualize the idea:

![multilayer](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse4.explicit.bing.net%2Fth%3Fid%3DOIP.oBTKz-elnata0w5Htvg95AHaD6%26pid%3DApi&f=1)

The image on the left (a) is an example of a single layer perceptron model while the image on the right (b) is an example of a multi layer perceptron model.

### Implementation
The implementation of the Multi-Layer Perceptron is as follows:
1. Initialize weights and biases
2. Forward propagation: feed the inputs forward into the function
3. Calculate the error
4. Backpropagation: want to minimize the error by taking the derivative/gradient of the error
5. Implement Stochastic Gradient Descent (discussed in Gradient Descent module)

### The Sigmoid Function?!
In the Logistic Regression module, we discussed the sigmoid function and its uses in logistic regression. However, the sigmoid function is also incredibly useful for deep neural networks. Because of its nonlinearity and easy differentiation, it makes for an ideal activation function.

### Backpropagation
Backpropagation is very important in many types of machine learning, including the multi-layer perceptron model. It is used to test points and minimize the error in order to find the best possible output given the inputs. Backpropagation is accomplished by taking the gradient of the error and using Stochastic Gradient Descent.

### TensorFlow
While we could hard-code all of the above steps, we will be using TensorFlow to implement this algorithm. TensorFlow is an open sourced library designed by Google that can complete a variety of tasks, but is made especially for deep neural networks, which is exactly what the multi-layer perceptron is. This is what makes it the ideal choice for coding.

# Task
In this module, instead of using a wine dataset, I will instead be using the fashion mnist dataset. This dataset classifies various pictures into different categories of clothing.



