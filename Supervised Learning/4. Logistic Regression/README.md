# Logistic Regression
In the Perceptron Model, we learned how to classify two objects. However, what happens when the data overlaps? Classification gets a lot harder. This is where logistic regression comes in. 

### Introduction to linearly separable vs. non-linearly separable 
![NonLinear](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmiro.medium.com%2Fmax%2F1542%2F1*5l08QfsUsrsOxcPzfDoStg.png&f=1&nofb=1)

Linearly separable means that the data is able to be completely separate. There is no overlap between the data and it is very easy to tell the different classes apart, as well as predict what class another object might belong to given certain attributes. However, non-linearly separable means that there is either overlap in the data  or the data can't be split by a linear line. Sometimes it might be easy to predict which class an unknown object belongs to, but other times it isn't so clear. Maybe the data is skewed towards the object being one class, but it could still be another class.

As an example, maybe you are trying to differentiate between red and white wine. Just through factors such as flavor and texture you can easily distinguish between the two types of wine. This is linearly separable data. However, it might not be as easy to tell the difference between different types of red wine. There can be significant overlap between the various types, as flavor and texture could be very similar. This is non-linearly separable data.

For linearly separable data, we can use the perceptron model and other similar models to perform classification. But how do we deal with non-linearly separable data? This is where logistic regression comes in.

### Logistic Regression Overview
Logistic regression deals with probabilities. Instead of saying that a object is definitely one class or another, it gives the probability that the object is a certain class. The most intuitive example could be talking about the weather. When the weatherman is predicting whether it will rain or not, he doesn't say "It definitely will rain" or "It definitely won't rain". Instead, he offers a percentage such as "There is a 40% chance of rain". What makes this example even more similar to machine learning is that the weatherman takes past data about various weather factors and compares the attributes to today's weather to make his prediction. In fact, weather services very likely use machine learning to make their predictions.

### Sigmoid Function
In order to make our predictions, we will use a sigmoid function as our activation function. Here is what the sigmoid function is: 
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fartificialintelligencestechnology.com%2Fwp-content%2Fuploads%2F2021%2F05%2Fsigmoid-function.png&f=1&nofb=1" width=50% height=50%>

When we graph the sigmoid function, we can see that it has a lot of nice properties that make it a very nice fit for logistic regression. First, the function ranges from 0 to 1, making it ideal for graphing probabilities. Second, it has a very nice, smooth S curve that gives percentages in a very logical manner. Finally, it is a relatively simple function to implement. Although there are many other logical choices of functions that can be used in logistic regression, we will focus on the sigmoid function. However, in my code, I will also try various other functions and see the results.

### Binary Cross Entropy Loss Function
In order to calculate the loss/error function, we will implement a version of the Bernoulli formula for binary probabilities to calculate loss. The general idea is that for binary probabilities, the probability (y) that a object is "x" means that the probability that the object is not "x" is 1-y. For the weather example, if there is a 70% chance that it will rain, then there is a 30% chance that it won't rain. Exact implementation of this code will be discussed more in depth within the code.

# Task
In this module I will perform logistic regression on multiple attribute of the load wine dataset in order to classify two classes of wine (Class 1 and 2). I will then compare to see how logistic regression performs using these different attributes.



