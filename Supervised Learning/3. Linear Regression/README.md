# Linear Regression
In the Perceptron Single Neuron Model, we did classification. This meant that we took various inputs and weighted them to decide what class/category the object should be put into. Now, through Linear Regression, we will be performing regression instead. This means that we will take multiple inputs are try to decide the best fit line.

### Example
Here is another wine example to illustrate the difference between classification and regression. Say we know the attributes of various classes of wine: fixed acidity, alcohol content, etc. If we wanted to perform classification, we might take these various attributes to determine what class of wine it was. This is what we did for the Perceptron Model: we took different attributes to determine whether it was class A or B wine. However, for regression, we are calculating best fit line. This means that when testing our model, we might take a fixed acidity to determine what the alcohol content is. If the data is relatively linear, the alcohol content should be close to the real alcohol content.

## Gradient Descent
In order to find the best fit line, we will perform gradient descent on our data to minimize the cost (or error) function. However, while in the gradient descent module we only explored the general idea about how gradient descent works, there are actually many different ways to perform gradient descent.

### Batch Gradient Descent
1. Start by selecting a learning rate and initial values.
2. Calculate the full gradient by calculating the gradient for all the training data
3. Compute [insert math equation here] to go in direction of minimum
4. Repeat steps 2-3 until a minimum is reached

Unfortunately, while batch gradient descent always finds the exact direction towards the minimum, it can be extremely slow, since you have to calculate the gradient for every single point. This can especially take a long time if you have a lot of data points. It is also unnecessary. This is where Stochastic Gradient Descent comes in.

### Stochastic Gradient Descent
1. Select a learning rate and initial values
2. Calculate the gradient for a single random data value.
3. Compute [insert math equation here] to go in direction of minimum
4. Repeat steps 2-3 until a minimum is reached

Stochastic Gradient Descent is often referred to as a drunk man stumbling his way home. While he may not always take the exact right steps towards home, he will eventually get there.

### Insert illustration here

### Things to do
Test how linear various data is?
Run time of stochastic vs. batch?
Upload stochastic vs. batch pictures from wikipedia
